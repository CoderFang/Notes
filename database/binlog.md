
参考链接：https://zhuanlan.zhihu.com/p/33504555

- binlog的作用:
1. 主从复制
2. 恢复数据

- binlog的日志格式：
> ROW / STATEMENT / MIXED


- 基于binlog的一主一从复制过程：
1. Master将数据的改变记录到binlog
2. Slave的IO进程连接到Master上，并请求从指定文件的指定位置之后的内容
3. Master收到Slave的IO进程请求后，Master上负责复制的IO将指定日志信息返回给Slave的IO进程（返回信息除了日志外，还有Master端binlog文件名及日志位置）
4. Slave的IO进程收到信息后，将接收到的日志内容依次添加到relay-log文件末端，并将Master的binlog文件名及位置记录到master-info文件中以便下次读取具体位置
5. Slave的sql进程检测到relay-log新增内容，会马上解析relay-log内容并执行
