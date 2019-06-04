#### Mysql面试题

> https://juejin.im/post/5cb6c4ef51882532b70e6ff0

- MySQL主从复制的流程和原理


- MySQL中MyIsam和InnoDB的区别（至少5点）


- InnoDB的4大特性

- InnoDB和MyIsam两者select count() 谁快，为什么？


- varchar和char的区别
1. varchar是变长，char是定长


- varchar(50)中的50涵义

- int(20)中的20的涵义

- 以上两个问题，为什么MySQL要这么设计？

- Mysql有多少种日志
1. 二进制日志（binlog）

2. 错误日志

3. 查询日志

4. 慢查询日志

5. redolog（InnoDB的事务日志）

6. undolog（InnoDB的事务日志）


- 事务的隔离级别
1. 读未提交
2. 读已提交
3. 可重复读
4. 可串行化


- MySQL的CPU飙升的处理（可能原因排查）
1. show processlist 查看进程，干掉

2. 查看超时日志和错误日志

> https://www.cnblogs.com/f-ck-need-u/archive/2018/05/08/9010872.html#auto_id_1


