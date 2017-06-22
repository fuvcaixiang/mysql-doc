# 创建数据库
1. 首先进入到mysql里面用命令 mysql -u root -p
2. 命令：create database <数据库名>
# 显示数据库
- 命令：use databases
# 删除数据库
- 命令：drop databases <数据库名> 
# 使用数据库
- 命令：use <数据库名>
# 创建数据表
- 命令：create table <表名> ( <字段名1> <类型1> [,..<字段名n> <类型n>]);
1. 学生信息表

  字段名    | 类型     | 空值  | 默认值   |  备注         
-----------|----------|----- |---------|---------
  sno      | int(4)   | NO   | NULL    | 主键
  sname    | char(20) | NO   | NULL    |                
  sex      | char(10) | NO   | F       |                
  sage     | int(4)   | NO   | NULL    |                
  sdeptno  | int(4)   | NO   | NULL    |               
  tag      | char(10) | YES  |  0      | 标志                
2. 课程信息表

 字段名   |  类型    | 空值  | 默认值    | 备注  
---------|----------|------|----------|---------
 cno     | int(4)   | NO   |  NULL    | 主键
 cname   | char(20) | NO   |  NULL    |        
 credit  | int(10)  | NO   |  NULL    |  
 3. 成绩信息表  

 字段名 |   类型     |  空值  |默认值  | 备注
-------|------------|-------|-------|-----------
 sno   | int(4)     | NO    | NULL  | 主键（参照学生表）    
 cno   | int(4)     | NO    | NULL  | 主键（参照课程表）
 grade | smallint(6)| YES   | NULL  |  
# 表结构
- ·查看表格结构命令：desc 表名
# 删除表
- 命令：drop table <表名>；
# 表插入数据
- 命令：insert into <表名> [( <字段名1>[,..<字段名n > ])] values ( 值1 )[, ( 值n )]
# 查询表中的数据
-  命令： select <字段1，字段2，...> from < 表名 > where < 表达式 >；
# 修改表中数据
- 命令：update 表名 set 字段=新值,... where 条件 ；
# 增加字段
命令：alter table 表名 add字段 类型 其他;
# 添加索引
- alter table 表名 add index 索引名 (字段名1[，字段名2 ...]);
