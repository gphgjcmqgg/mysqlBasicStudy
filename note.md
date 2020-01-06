# mysqlBasicStudy

## mysql默认端口号

mysql 服务默认端口号 3306

## 服务启动和停止

net stop 服务名
net start 服务名

## mysql服务登陆

mysql -h localhost -P 3306 -u root -p

## mysql常见命令

1. 查看当前所有数据库
show databases;
2. 打开指定库
use test;
3. 查看当前库的所有表
show tables;
4. 查看其他库的所有表
show tables from 库名;
5. 创建表
create table 表名(
  列名 列类型，
  列名 列类型，
  ...
)
6. 查看表结构
desc 表名;
7. 查看服务器的版本
--登陆mysql服务端
select version();
--dos状态
mysql --version
mysql -V
8. 查看所在数据库
select database();

## mysql注释

单行：#注释文字
单行：-- 注释文字
多行：/*  注释文字   */
