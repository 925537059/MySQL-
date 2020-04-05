## 一、介绍对数据库操作相关的命令
### 1、创建一个新的数据库
```SQL
create database databasetest;
```      
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/1.png?raw=true)
### 2、查看和选择数据库
```SQL
show databases;
use databasetest;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/2.png?raw=true)
### 3、删除数据库
```SQL
drop database databasetest;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/3.png?raw=true)
## 二、如何查看MySQL数据库中的引擎
### 1、查看所支持的存储引擎
```SQL
show engines;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/4.png?raw=true) 
### 2、查看默认的存储引擎
```SQL 
show variables like '%storage_engine%';
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/5.png?raw=true) 
## 三、介绍对表操作的相关指令
### 1、在数据库中创建一个新的表
```SQL
CREATE TABLE t_dept(
 	deptno INT,
	dname VARCHAR(20),
	loc VARCHAR(40)
	); 
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/7.png?raw=true)
### 2、查看表的定义信息
```SQL
describe t_debt;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/7.png?raw=true) 
### 3、删除表
```SQL
drop table t_dept;
describe t_dept;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/8.png?raw=true)
### 4、修改表名
```SQL
ALTER TABLE t_dept RENAME t_dept1;
show table;
describe t_dept1;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/9.png?raw=true) 
### 5、增加字段和删除字段
#### 在表的最后面增加字段
```SQL
alter table t_dept1
add tel varchar(20);
describe t_dept1;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/10.png?raw=true) 
#### 在表指定字段后增加字段
```SQL
alter table t_dept1
add bname varchar(10)
after dname;
describe t_dept1;
```
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/11.png?raw=true)
#### 删除字段
```SQL
alter table t_dept1
drop bname;
describe t_dept1;
![](https://github.com/BiubiuOoo/Homework-of-MySQL/blob/master/images/12.png?raw=true)
### 四、










