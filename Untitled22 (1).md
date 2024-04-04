```python
create table AI_tool(id int,technology varchar(40));
Query OK, 0 rows affected (0.04 sec)

mysql> insert into AI_tool values(1,'DS'),(1,'tableau'),(1,'sql'),(2 ,'R'),(2,'power bi'),(1,'python');
Query OK, 6 rows affected (0.01 sec)
Records: 6  Duplicates: 0  Warnings: 0

mysql> select *from AI_tool;
+------+------------+
| id   | technology |
+------+------------+
|    1 | DS         |
|    1 | tableau    |
|    1 | sql        |
|    2 | R          |
|    2 | power bi   |
|    1 | python     |
+------+------------+

mysql> select *from AI_tool where technology in('DS','tableau','sql','python');
+------+------------+
| id   | technology |
+------+------------+
|    1 | DS         |
|    1 | tableau    |
|    1 | sql        |
|    1 | python     |
+------+------------+
4 rows in set (0.00 sec)

mysql>select *from user;
+------+------+------------+
| id   | p_id | p_l        |
+------+------+------------+
|    1 | 1001 | 2024-03-12 |
|    2 | 1003 | 2024-03-11 |
+------+------+------------+
2 rows in set (0.00 sec)

mysql> select *from pro_info;
+------+-----------+
| p_id | p_name    |
+------+-----------+
| 1001 | blog      |
| 1002 | youtube   |
| 1003 | education |
+------+-----------+
3 rows in set (0.00 sec)

mysql> select p.p_id from pro_info as p left join user as u on p.p_id=u.p_id where u.p_l is null;
+------+
| p_id |
+------+
| 1002 |
+------+
1 row in set (0.00 sec)





```
