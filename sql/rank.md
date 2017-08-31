## rank()函数和 over()函数的使用
### rank() over(order by 列名 排序) 的结果是不连续的，如果有4个人，其中有3个是并列第1名，那么最后的排序结果结果如：1 1 1 4;
### 举个栗子  
```SQL
1. SELECT COLA , RANK( ) OVER(order by COLE ASC )  E  FROM TABLE_A ;
```
### 结果如下:
![上述SQL执行结果](https://github.com/2629743986/StudyNote/blob/master/sql/rank().png)
### 注意 E 字段的排名顺序
