<h1>limit(重点中的重点)

前提：limit是mysql特有的，其他数据库中没有，不通用。

作用：limit取结果集的部分数据

语法机制：

​	limit startIndex ,length

​	startIndex表示起始位置(0代表第一个数据)；

​	length表示取多少个

注意：limit 是sql语句中最后执行的一个环节

eg：取出工资前五名的员工(思路：降序排取前五)

```sql
select ename,sal from emp order by sal desc limit 3,6;
```



