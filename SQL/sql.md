

## 语法
```{sql}
select * from websites;
```
语句末尾要有分号

* 一些最重要的sql命令
  select, update ,delete , insert into, create table , alter database, create database,

## select
选择指定列
```{sql}
select column1,column2,... from table_name;
```
选择所有列
```{sql}
select * from table_name
```

## select distinct 
返回唯一不同的值,相当于转成集合
```{sql}
select distince column1,column2,... from table_name
```

## where
过滤记录,用于提取满足指定条件的记录
```{sql}
select column1,column2,... from table_name where condition;
```
```{sql}
select * from websites where country='CN'
```
* where 语句中运算符
  <> 不等于,between 某个范围内, like 某种模式, in 针对某个列的多个可能值

## and or
```{sql}
SELECT * FROM Websites
WHERE country='CN' AND alexa > 50;
```
```{sql}
select * from web where alexa>15 and (country='CN' or country='USA)
```

## order by
对结果集进行排序
```{sql}
select column1,column2,... from tabel order by column1,column2,... asc|desc;
```
* asc 升序排序
* desc 降序排序

## insert into
往已有数据表中插入新行
```{sql}
insert into table_name (column1,column2,...)
values (value1,value2,...);
```
或者不指定插入的列名
```{sql}
insert into tabel_name 
values (value1,value2,...);
```

## update
更新数据表中某些数据
```{sql}
update table_name
set column1=value1,column2=value2,...
where condition;
```
```{sql}

```
