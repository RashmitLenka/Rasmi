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

mysql>





```
