<h1>结果集相加

eg:找出岗位是selesman和manager的员工

```sql
select ename,job from emp where job = 'manager'
union
select ename,job from emp where job = 'salesman';
```



两张不相干的表中的数据拼接在一起显示

```sql
select * from emp
union
select * from dept;#第一个查询结果集列的数量必须与第二个查询结果集的数量一致
```

