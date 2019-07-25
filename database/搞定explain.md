
#### MySQL Explain

- 参考连接：
1. [MySQL Explain](https://segmentfault.com/a/1190000008131735)

##### 执行explain返回的字段
- id
> select查询的标识符

- select_type
1. SIMPLE
2. PRIMARY,
3. UNION,
4. DEPENDENT UNION,
5. UNION RESULT,
6. SUBQUERY,
7. DEPENDENT SUBQUERY

3. table 

4. partitions

5. type

6. possible_keys

7. key
8. key_len
9. ref
10. row
11. filtered
12. Extra