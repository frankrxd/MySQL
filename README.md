### 1.四个基本概念

* 数据、数据库、数据库管理系统、数据库系统

* 数据库是长期储存在计算机内、有组织、可共享的大量数据的集合。数据库中的数据按一定数据模型组织、描述和储存，具有较小的冗余度、较高的数据独立性和易拓展性，并可为各种用户共享



### 2.数据库管理系统（DBMS）

主要功能：

- 数据定义功能：DDL语音
- 数据操纵功能：DML语音
- 数据库运行管理
- 提供方便有效地存取数据库信息的接口和工具
- 数据库的建立和维护功能	



### 3.SQL语言

SQL是一种数据库查询和程序设计语言，用于存取数据以及查询、更新和管理关系数据库系统

SQL 具有如下优点。

- 一体化：SQL 集数据定义、数据操作和数据控制于一体，可以完成数据库中的全部工作。
- 使用方式灵活：SQL 具有两种使用方式，可以直接以命令方式交互使用；也可以嵌入使用，嵌入C、[C++](http://c.biancheng.net/cplus/)、Fortran、COBOL、Java 等语言中使用。
- 非过程化：只提操作要求，不必描述操作步骤，也不需要导航。使用时只需要告诉计算机“做什么”，而不需要告诉它“怎么做”，存储路径的选择和操作的执行由数据库管理系统自动完成。
- 语言简洁、语法简单：该语言的语句都是由描述性很强的英语单词组成，而且这些单词的数目不多。

SQL 包含以下 4 部分：

- 数据定义语言（DDL）：DROP、CREATE、ALTER 等语句。
- 数据操作语言（DML）：INSERT（插入）、UPDATE（修改）、DELETE（删除）语句。
- 数据查询语言（DQL）：SELECT 语句。
- 数据控制语言（DCL）: GRANT、REVOKE、COMMIT、ROLLBACK 等语句。



### 4.数据库访问接口

- ODBC：开放数据库互联
- JDBC：JAVA数据库连接
- ADO.NET：NET 框架下开发设计的一组用于和数据源进行交互的面向对象类库。
- PDO：为 PHP 访问数据库定义了一个轻量级的、一致性的接口，它提供了一个数据访问抽象层，这样，无论使用什么数据库，都可以通过一致的函数执行查询和获取数据。



### 5.MySQL系统特性

- 使用 C 和 [C++](http://c.biancheng.net/cplus/) 编写，并使用多种编译器进行测试，保证源代码的可移植性。
- 支持 AIX、FreeBSD、HP-UX、Linux、Mac OS、NovellNetware、OpenBSD、OS/2 Wrap、Solaris、Windows 等多种操作系统。
- 为多种编程语言提供了 API。这些编程语言包括 C、C++、[Python](http://c.biancheng.net/python/)、[Java](http://c.biancheng.net/java/)、Perl、PHP、Eiffel、Ruby 和 Tcl 等。
- 支持多线程，充分利用 CPU 资源。
- 优化的 SQL 查询算法，有效地提高查询速度。
- 既能够作为一个单独的应用程序应用在客户端服务器网络环境中，也能够作为一个库而嵌入其他的软件中。
- 提供多语言支持，常见的编码如中文的 GB 2312、BIG 5，日文的 Shift_JIS 等都可以用作数据表名和数据列名。
- 提供 TCP/IP、ODBC 和 JDBC 等多种数据库连接途径。
- 提供用于管理、检查、优化数据库操作的管理工具。
- 支持大型的数据库。可以处理拥有上千万条记录的大型数据库。
- 支持多种存储引擎。



### 6.MySQL 5.7新特性

- 随机root密码：MySQL 5.7 数据库初始化完成后，会自动生成一个 root@localhost 用户，root 用户的密码不为空，而是随机产生一个密码。
- 自定义test数据库：MySQL 5.7 默认安装完成后没有 test 数据库。用户可以自行创建 test 数据库并对其进行权限控制。
- 默认SSL加密：MySQL 5.7 采用了更加简单的 SSL 安全访问机制，默认连接使用 SSL 的加密方式。
- 密码过期策略：MySQL 5.7 支持用户设置密码过期策略，要求用户在一定时间过后必须修改密码。
- 用户锁：MySQL 5.7 为管理员提供了暂时禁用某个用户的功能，使被锁定的用户无法访问和使用数据库。
- 全面支持JSON：MySQL 5.7 也提供了对 JSON 的支持，在服务器端提供了一组便于操作 JSON 的函数。存储的方法是将 JSON 编码成 BLOB 后再由存储引擎进行处理。这样，MySQL 就同时拥有了关系型数据库和非关系型数据库的优点，并且可以提供完整的事务支持。
- 支持两类生成列：生成列是通过数据库中的其他列计算得到的一列。当为生成列创建索引时，可以便捷地加快查询速度。MySQL 5.7 支持虚拟生成列和存储生成列。虚拟生成列仅将数据保存在表的元数据中，作为缺省的生成列类型；存储生成列则是将数据永久保存在磁盘上，需要更多的磁盘空间。
- 引入系统库：系统库中包含一系列视图、函数和存储过程，通过多线程、多进程、组合事务提交和基于行的优化方式将复制功能提高 5 倍以上，用户向外扩充其跨商品系统的工作负载时，得以大幅提升复制的效能和效率。



### 7.MySQL服务端实用工具

- mysqld：SQL 后台程序（即 MySQL 服务器进程）。该程序必须运行之后，客户端才能通过连接服务器来访问数据库。
- mysqld_safe：服务器启动脚本。在 UNIX 和 NewWare 中推荐使用 mysqld_safe 来启动 mysqld 服务器。mysqld_safe 增加了一些安全性，例如，当出现错误时，重启服务器并向错误日志文件中写入运行时间信息。
- mysql.server：服务器启动脚本。该脚本用于使用包含为特定级别的、运行启动服务器脚本的、运行目录的系统。它调用 mysqld_safe 来启动 MySQL 服务器。
- mysqld_multi：服务器启动脚本，可以启动或停止系统上安装的多个服务器。
- mysamchk：用来描述、检查、优化和维护 MyISAM 表的实用工具。
- mysqlbug：MySQL 缺陷报告脚本。它可以用来向 MySQL 邮件系统发送缺陷报告。
- mysql_install_db：该脚本用默认权限创建 MySQL 授予权表。通常只是在系统上首次安装 MySQL 时执行一次。



### 8.MySQl客户端实用工具

- myisampack：压缩 MyISAM 表以产生更小的只读表的一个工具.
- mysql：交互式输入 SQL 语句或从文件经批处理模式执行它们的命令行工具。
- mysqlacceess：检查访问主机名、用户名和数据库组合的权限的脚本。
- mysqladmin：执行管理操作的客户程序，例如创建或删除数据库、重载授权表、将表刷新到硬盘上以及重新打开日志文件。Mysqladmin 还可以用来检索版本、进程以及服务器的状态信息。
- mysqlbinlog：从二进制日志读取语句的工具。在二进制日志文件中包含执行过的语句，可用来帮助系统从崩溃中恢复。
- mysqlcheck：检查、修复、分析以及优化表的表维护客户程序。
- mysqldump：将 MySQL 数据库转储到一个文件（例如 SQL 语句或 Tab 分隔符文本文件）的客户程序。
- mysqlhotcopy：当服务器在运行时，快速备份 MyISAM 或 ISAM 表的工具。
- mysql import：使用 LOAD DATA INFILE 将文本文件导入相应的客户程序。
- mysqlshow：显示数据库、表、列以及索引相关信息的客户程序。
- perror：显示系统或 MySQL 错误代码含义的工具。

* show variables like '%datadir%'; 显示数据库文件路径。

### 9.MySQL存储引擎

| 功能         | MylSAM | MEMORY | InnoDB | Archive |
| ------------ | ------ | ------ | ------ | ------- |
| 存储限制     | 256TB  | RAM    | 64TB   | None    |
| 支持事务     | No     | No     | Yes    | No      |
| 支持全文索引 | Yes    | No     | No     | No      |
| 支持树索引   | Yes    | Yes    | Yes    | No      |
| 支持哈希索引 | No     | Yes    | No     | No      |
| 支持数据缓存 | No     | N/A    | Yes    | No      |
| 支持外键     | No     | No     | Yes    | No      |

可以根据以下的原则来选择 MySQL 存储引擎：

- 如果要提供提交、回滚和恢复的事务安全（ACID 兼容）能力，并要求实现并发控制，InnoDB 是一个很好的选择。
- 如果数据表主要用来插入和查询记录，则 MyISAM 引擎提供较高的处理效率。
- 如果只是临时存放数据，数据量不大，并且不需要较高的数据安全性，可以选择将数据保存在内存的 MEMORY 引擎中，MySQL 中使用该引擎作为临时表，存放查询的中间结果。
- 如果只有 INSERT 和 SELECT 操作，可以选择Archive 引擎，Archive 存储引擎支持高并发的插入操作，但是本身并不是事务安全的。Archive 存储引擎非常适合存储归档数据，如记录日志信息可以使用 Archive 引擎。

```mysql
SET default_storage_engine=< 存储引擎名 >
```



### 10.MySql数据类型

* 数值类型：整数类型包括 TINYINT、SMALLINT、MEDIUMINT、INT、BIGINT，浮点数类型包括 FLOAT 和 DOUBLE，定点数类型为 DECIMAL。

* 日期/时间类型：包括 YEAR、TIME、DATE、DATETIME 和 TIMESTAMP。
*  字符串类型：包括 CHAR、VARCHAR、BINARY、VARBINARY、BLOB、TEXT、ENUM 和 SET 等。
* 二进制类型：包括 BIT、BINARY、VARBINARY、TINYBLOB、BLOB、MEDIUMBLOB 和 LONGBLOB。

| 类型名称      | 说明           | 存储需求 |
| ------------- | -------------- | -------- |
| TINYINT       | 很小的整数     | 1个字节  |
| SMALLINT      | 小的整数       | 2个宇节  |
| MEDIUMINT     | 中等大小的整数 | 3个字节  |
| INT (INTEGHR) | 普通大小的整数 | 4个字节  |
| BIGINT        | 大整数         | 8个字节  |

| 类型名称      | 说明                                      | 存储需求                |
| ------------- | ----------------------------------------- | ----------------------- |
| TINYINT       | -128〜127                                 | 0 〜255                 |
| SMALLINT      | -32768〜32767                             | 0〜65535                |
| MEDIUMINT     | -8388608〜8388607                         | 0〜16777215             |
| INT (INTEGER) | -2147483648〜2147483647                   | 0〜4294967295           |
| BIGINT        | -9223372036854775808〜9223372036854775807 | 0〜18446744073709551615 |

| 类型名称            | 说明               | 存储需求   |
| ------------------- | ------------------ | ---------- |
| FLOAT               | 单精度浮点数       | 4 个字节   |
| DOUBLE              | 双精度浮点数       | 8 个字节   |
| DECIMAL (M, D)，DEC | 压缩的“严格”定点数 | M+2 个字节 |

| 类型名称  | 日期格式            | 日期范围                                          | 存储需求 |
| --------- | ------------------- | ------------------------------------------------- | -------- |
| YEAR      | YYYY                | 1901 ~ 2155                                       | 1 个字节 |
| TIME      | HH:MM:SS            | -838:59:59 ~ 838:59:59                            | 3 个字节 |
| DATE      | YYYY-MM-DD          | 1000-01-01 ~ 9999-12-3                            | 3 个字节 |
| DATETIME  | YYYY-MM-DD HH:MM:SS | 1000-01-01 00:00:00 ~ 9999-12-31 23:59:59         | 8 个字节 |
| TIMESTAMP | YYYY-MM-DD HH:MM:SS | 1980-01-01 00:00:01 UTC ~ 2040-01-19 03:14:07 UTC | 4 个字节 |

| 类型名称   | 说明                                         | 存储需求                                                   |
| ---------- | -------------------------------------------- | ---------------------------------------------------------- |
| CHAR(M)    | 固定长度非二进制字符串                       | M 字节，1<=M<=255                                          |
| VARCHAR(M) | 变长非二进制字符串                           | L+1字节，在此，L< = M和 1<=M<=255                          |
| TINYTEXT   | 非常小的非二进制字符串                       | L+1字节，在此，L<2^8                                       |
| TEXT       | 小的非二进制字符串                           | L+2字节，在此，L<2^16                                      |
| MEDIUMTEXT | 中等大小的非二进制字符串                     | L+3字节，在此，L<2^24                                      |
| LONGTEXT   | 大的非二进制字符串                           | L+4字节，在此，L<2^32                                      |
| ENUM       | 枚举类型，只能有一个枚举字符串值             | 1或2个字节，取决于枚举值的数目 (最大值为65535)             |
| SET        | 一个设置，字符串对象可以有零个或 多个SET成员 | 1、2、3、4或8个字节，取决于集合 成员的数量（最多64个成员） |

| 插入值   | CHAR(4) | 存储需求 | VARCHAR(4) | 存储需求 |
| -------- | ------- | -------- | ---------- | -------- |
| ' '      | '  '    | 4字节    | ''         | 1字节    |
| 'ab'     | 'ab '   | 4字节    | 'ab'       | 3字节    |
| 'abc'    | 'abc '  | 4字节    | 'abc'      | 4字节    |
| 'abcd'   | 'abcd'  | 4字节    | 'abcd'     | 5字节    |
| 'abcdef' | 'abcd'  | 4字节    | 'abcd'     | 5字节    |

| 类型名称       | 说明                 | 存储需求               |
| -------------- | -------------------- | ---------------------- |
| BIT(M)         | 位字段类型           | 大约 (M+7)/8 字节      |
| BINARY(M)      | 固定长度二进制字符串 | M 字节                 |
| VARBINARY (M)  | 可变长度二进制字符串 | M+1 字节               |
| TINYBLOB (M)   | 非常小的BLOB         | L+1 字节，在此，L<2^8  |
| BLOB (M)       | 小 BLOB              | L+2 字节，在此，L<2^16 |
| MEDIUMBLOB (M) | 中等大小的BLOB       | L+3 字节，在此，L<2^24 |
| LONGBLOB (M)   | 非常大的BLOB         | L+4 字节，在此，L<2^32 |



### 11.MySQL常用运算符

| 算术运算符 | 说明               |
| ---------- | ------------------ |
| +          | 加法运算           |
| -          | 减法运算           |
| *          | 乘法运算           |
| /          | 除法运算，返回商   |
| %          | 求余运算，返回余数 |



| 比较运算符        | 说明                               |
| ----------------- | ---------------------------------- |
| =                 | 等于                               |
| <                 | 小于                               |
| <=                | 小于等于                           |
| >                 | 大于                               |
| >=                | 大于等于                           |
| <=>               | 安全的等于，不会返回 UNKNOWN       |
| <> 或!=           | 不等于                             |
| IS NULL 或 ISNULL | 判断一个值是否为 NULL              |
| IS NOT NULL       | 判断一个值是否不为 NULL            |
| LEAST             | 当有两个或多个参数时，返回最小值   |
| GREATEST          | 当有两个或多个参数时，返回最大值   |
| BETWEEN AND       | 判断一个值是否落在两个值之间       |
| IN                | 判断一个值是IN列表中的任意一个值   |
| NOT IN            | 判断一个值不是IN列表中的任意一个值 |
| LIKE              | 通配符匹配                         |
| REGEXP            | 正则表达式匹配                     |



| 逻辑运算符   | 说明     |
| ------------ | -------- |
| NOT 或者 !   | 逻辑非   |
| AND 或者 &&  | 逻辑与   |
| OR 或者 \|\| | 逻辑或   |
| XOR          | 逻辑异或 |



| 位运算符 | 说明                   |
| -------- | ---------------------- |
| \|       | 按位或                 |
| &        | 按位与                 |
| ^        | 按位异或               |
| <<       | 按位左移               |
| >>       | 按位右移               |
| ~        | 按位取反，反转所有比特 |



| 优先级由低到高排列 | 运算符                                                       |
| ------------------ | ------------------------------------------------------------ |
| 1                  | =(赋值运算）、:=                                             |
| 2                  | II、OR                                                       |
| 3                  | XOR                                                          |
| 4                  | &&、AND                                                      |
| 5                  | NOT                                                          |
| 6                  | BETWEEN、CASE、WHEN、THEN、ELSE                              |
| 7                  | =(比较运算）、<=>、>=、>、<=、<、<>、!=、 IS、LIKE、REGEXP、IN |
| 8                  | \|                                                           |
| 9                  | &                                                            |
| 10                 | <<、>>                                                       |
| 11                 | -(减号）、+                                                  |
| 12                 | *、/、%                                                      |
| 13                 | ^                                                            |
| 14                 | -(负号）、〜（位反转）                                       |
| 15                 | !                                                            |



### *.MySQL常用操作

#### 1.创建数据库[CREATE DATABASE]

```Mysql
CREATE DATABASE [IF NOT EXISTS] <数据库名>
 [[DEFAULT] CHARACTER SET <字符集名>] 
 [[DEFAULT] COLLATE <校对规则名>];
 #eg1：
 mysql> CREATE DATABASE test_db;
 #eg2：
 mysql> CREATE DATABASE IF NOT EXISTS test_db_char
    -> DEFAULT CHARACTER SET utf8
    -> DEFAULT COLLATE utf8_chinese_ci;
```



#### 2.查看数据库[SHOW DATABASES]

```Mysql
SHOW DATABASES [LIKE '数据库名'];
#eg1：
SHOW DATABASES LIKE 'test_db';
#eg2：
SHOW DATABASES LIKE '%test%';
#eg3：
SHOW DATABASES LIKE 'db%';
#eg4：
SHOW DATABASES LIKE '%db';
```



#### 3.修改数据库[ALTER DATABASE]

```Mysql
ALTER DATABASE [数据库名] {  
[ DEFAULT ] CHARACTER SET <字符集名> | 
[ DEFAULT ] COLLATE <校对规则名>}
```



#### 4.删除数据库[DROP DATABASE]

```Mysql
DROP DATABASE [ IF EXISTS ] <数据库名>；
```



#### 5.选择数据库[USE]

```mysql
USE <数据库名>；
```



#### 6.创建数据表[CREATE TABLE]

````mysql
CREATE TABLE <表名> ([表定义选项])[表选项][分区选项];
#表定义选项
<列名1> <类型1> [,…] <列名n> <类型n>
#查看表结构
DESCRIBE <表名>;#DESC <表名>;
SHOW CREATE TABLE <表名>\G；

````



#### 7.修改数据表[ALTER TABLE]

````mysql
ALTER TABLE <表名> [修改选项]
#修改选项
{ ADD COLUMN <列名> <类型>
| CHANGE COLUMN <旧列名> <新列名> <新列类型>
| ALTER COLUMN <列名> { SET DEFAULT <默认值> | DROP DEFAULT }
| MODIFY COLUMN <列名> <类型>
| DROP COLUMN <列名>
| RENAME TO <新表名>
| ALTER TABLE <表名> CHANGE <旧字段名> <新字段名> <新数据类型> }
````



#### 8.删除数据表[DROP TABLE]

````mysql
DROP TABLE [IF EXISTS] 表名1 [ ,表名2, 表名3 ...]
````



#### 9.主键[PRIMARY KEY]

主键约束即在表中定义一个主键来唯一确定表中每一行数据的标识符。主键可以是表中的某一列或者多列的组合，其中由多列组合的主键称为复合主键。主键应该遵守下面的规则：

- 每个表只能定义一个主键。
- 主键值必须唯一标识表中的每一行，且不能为 NULL，即表中不可能存在两行数据有相同的主键值。这是唯一性原则。
- 一个列名只能在复合主键列表中出现一次。
- 复合主键不能包含不必要的多余列。当把复合主键的某一列删除后，如果剩下的列构成的主键仍然满足唯一性原则，那么这个复合主键是不正确的。这是最小化原则。

````mysql
#在定义列的同时指定主键
<字段名> <数据类型> PRIMARY KEY [默认值]
#eg:
mysql> CREATE TABLE tb_emp3
    -> (
    -> id INT(11) PRIMARY KEY,
    -> name VARCHAR(25),
    -> deptId INT(11),
    -> salary FLOAT
    -> );

#定义完所有列之后，指定主键的语法格式
[CONSTRAINT <约束名>] PRIMARY KEY [字段名]
#eg:
mysql> CREATE TABLE tb_emp4
    -> (
    -> id INT(11),
    -> name VARCHAR(25),
    -> deptId INT(11),
    -> salary FLOAT,
    -> PRIMARY KEY(id)
    -> );

#创建表时设置复合主键
PRIMARY KEY [字段1，字段2，…,字段n]
#eg：
mysql> CREATE TABLE tb_emp5
    -> (
    -> name VARCHAR(25),
    -> deptId INT(11),
    -> salary FLOAT,
    -> PRIMARY KEY(id,deptId)
    -> );
    
#修改表时添加主键约束
ALTER TABLE <数据表名> ADD PRIMARY KEY(<列名>);
#eg:
mysql> ALTER TABLE tb_emp2
    -> ADD PRIMARY KEY(id);
````



#### 10.外键[FOREIGN KEY]

外键约束（FOREIGN KEY）用来在两个表的数据之间建立链接，它可以是一列或者多列。一个表可以有一个或多个外键。

定义一个外键时，需要遵守下列规则：

- 父表必须已经存在于数据库中，或者是当前正在创建的表。如果是后一种情况，则父表与子表是同一个表，这样的表称为自参照表，这种结构称为自参照完整性。
- 必须为父表定义主键。
- 主键不能包含空值，但允许在外键中出现空值。也就是说，只要外键的每个非空值出现在指定的主键中，这个外键的内容就是正确的。
- 在父表的表名后面指定列名或列名的组合。这个列或列的组合必须是父表的主键或候选键。
- 外键中列的数目必须和父表的主键中列的数目相同。
- 外键中列的数据类型必须和父表主键中对应列的数据类型相同。

````mysql
#创建表时设置外键约束
[CONSTRAINT <外键名>] FOREIGN KEY 字段名 [，字段名2，…]
REFERENCES <主表名> 主键列1 [，主键列2，…]
#eg:
mysql> CREATE TABLE tb_dept1
    -> (
    -> id INT(11) PRIMARY KEY,
    -> name VARCHAR(22) NOT NULL,
    -> location VARCHAR(50)
    -> );
mysql> CREATE TABLE tb_emp6
    -> (
    -> id INT(11) PRIMARY KEY,
    -> name VARCHAR(25),
    -> deptId INT(11),
    -> salary FLOAT,
    -> CONSTRAINT fk_emp_dept1
    -> FOREIGN KEY(deptId) REFERENCES tb_dept1(id)
    -> );

#修改表时添加外键约束
ALTER TABLE <数据表名> ADD CONSTRAINT <索引名>
FOREIGN KEY(<列名>) REFERENCES <主表名> (<列名>);
#eg：
mysql> ALTER TABLE tb_emp2
    -> ADD CONSTRAINT fk_tb_dept1
    -> FOREIGN KEY(deptId)
    -> REFERENCES tb_dept1(id);

#删除外键约束
ALTER TABLE <表名> DROP FOREIGN KEY <外键约束名>;
#eg：
mysql> ALTER TABLE tb_emp2
    -> DROP FOREIGN KEY fk_tb_dept1;
    
````



#### 11.唯一约束[UNIQUE]

唯一约束（Unique Key）要求该列唯一，允许为空，但只能出现一个空值。唯一约束可以确保一列或者几列不出现重复值。

````mysql
#创建表时设置唯一约束
<字段名> <数据类型> UNIQUE
#eg：
mysql> CREATE TABLE tb_dept2
    -> (
    -> id INT(11) PRIMARY KEY,
    -> name VARCHAR(22) UNIQUE,
    -> location VARCHAR(50)
    -> );

#修改表时添加唯一约束
ALTER TABLE <数据表名> ADD CONSTRAINT <唯一约束名> UNIQUE(<列名>);
#eg：
mysql> ALTER TABLE tb_dept1
    -> ADD CONSTRAINT unique_name UNIQUE(name);.

#删除唯一约束
ALTER TABLE <表名> DROP INDEX <唯一约束名>;
#eg：
mysql> ALTER TABLE tb_dept1
    -> DROP INDEX unique_name;
````



#### 12.检查约束[CHECK]

检查约束（CHECK）可以通过 CREATE TABLE 或 ALTER TABLE 语句实现，根据用户实际的完整性要求来定义。它可以分别对列或表实施 CHECK 约束。

````mysql
CHECK <表达式>
#创建时设置检查约束
CHECK(<检查约束>)
#eg：
mysql> CREATE TABLE tb_emp7
    -> (
    -> id INT(11) PRIMARY KEY,
    -> name VARCHAR(25),
    -> deptId INT(11),
    -> salary FLOAT,
    -> CHECK(salary>0 AND salary<100),
    -> FOREIGN KEY(deptId) REFERENCES tb_dept1(id)
    -> );
    
#修改时添加检查约束
ALTER TABLE tb_emp7 ADD CONSTRAINT <检查约束名> CHECK(<检查约束>)
mysql> ALTER TABLE tb_emp7
    -> ADD CONSTRAINT check_id
    -> CHECK(id>0);
    
#删除检查约束
ALTER TABLE <数据表名> DROP CONSTRAINT <检查约束名>;
````



#### 13.默认值约束[Default]

“默认值（Default）”的完整称呼是“默认值约束（Default Constraint）”。MySQL默认值约束用来指定某列的默认值。

````mysql
#创建时设置默认值约束
<字段名> <数据类型> DEFAULT <默认值>;
#eg：
mysql> CREATE TABLE tb_dept3
    -> (
    -> id INT(11) PRIMARY KEY,
    -> name VARCHAR(22),
    -> location VARCHAR(50) DEFAULT 'Beijing'
    -> );

#修改时添加默认值约束
ALTER TABLE <数据表名>
CHANGE COLUMN <字段名> <数据类型> DEFAULT <默认值>;
#eg：
mysql> ALTER TABLE tb_dept3
    -> CHANGE COLUMN location
    -> location VARCHAR(50) DEFAULT 'Shanghai';

#删除默认值约束
ALTER TABLE <数据表名>
CHANGE COLUMN <字段名> <字段名> <数据类型> DEFAULT NULL;
#eg：
mysql> ALTER TABLE tb_dept3
    -> CHANGE COLUMN location
    -> location VARCHAR(50) DEFAULT NULL;
````



#### 14.非空约束[NOT NULL]

非空约束（NOT NULL）可以通过 CREATE TABLE 或 ALTER TABLE 语句实现。在表中某个列的定义后加上关键字 NOT NULL 作为限定词，来约束该列的取值不能为空。

````mysql
#创建时设置非空约束
<字段名> <数据类型> NOT NULL;
eg：
mysql> CREATE TABLE tb_dept4
    -> (
    -> id INT(11) PRIMARY KEY,
    -> name VARCHAR(22) NOT NULL,
    -> location VARCHAR(50)
    -> );

#修改时
ALTER TABLE <数据表名>
CHANGE COLUMN <字段名>
<字段名> <数据类型> NOT NULL;
#eg：
mysql> ALTER TABLE tb_dept4
    -> CHANGE COLUMN location
    -> location VARCHAR(50) NOT NULL;

#删除时
ALTER TABLE <数据表名>
CHANGE COLUMN <字段名> <字段名> <数据类型> NULL;
#eg：
mysql> ALTER TABLE tb_dept4
    -> CHANGE COLUMN location
    -> location VARCHAR(50) NULL;
````



#### 15.查看表中约束

同查看数据表.



#### 16.查询数据表[SELECT]

表单查询是指从一张表的数据中查询所需的数据，主要有查询所有字段、查询指定字段、查询指定记录、查询空值、多条件的查询、对查询结果进行排序等。

* select基本语法：

  ````mysql
  SELECT
  {* | <字段列名>}
  [
  FROM <表 1>, <表 2>…
  [WHERE <表达式>
  [GROUP BY <group by definition>
  [HAVING <expression> [{<operator> <expression>}…]]
  [ORDER BY <order by definition>]
  [LIMIT[<offset>,] <row count>]
  ]
  
  #{*|<字段列名>}包含星号通配符的字段列表，表示查询的字段，其中字段列至少包含一个字段名称，如果要查询多个字段，多个字段之间要用逗号隔开，最后一个字段后不要加逗号。
  #FROM <表 1>，<表 2>…，表 1 和表 2 表示查询数据的来源，可以是单个或多个。
  #WHERE 子句是可选项，如果选择该项，将限定查询行必须满足的查询条件。
  #GROUP BY< 字段 >，该子句告诉 MySQL 如何显示查询出来的数据，并按照指定的字段分组。
  #[ORDER BY< 字段 >]，该子句告诉 MySQL 按什么样的顺序显示查询出来的数据，可以进行的排序有升序（ASC）和降序（DESC）。
  #[LIMIT[<offset>，]<row count>]，该子句告诉 MySQL 每次显示查询出来的数据条数。
  ````

* 使用“*”查询表中全部内容

  ````mysql
  SELECT * FROM 表名;
  #eg：
  mysql> use test_db;
  Database changed
  mysql> SELECT * FROM tb_students_info;
  +----+--------+---------+------+------+--------+------------+
  | id | name   | dept_id | age  | sex  | height | login_date |
  +----+--------+---------+------+------+--------+------------+
  |  1 | Dany   |       1 |   25 | F    |    160 | 2015-09-10 |
  |  2 | Green  |       3 |   23 | F    |    158 | 2016-10-22 |
  |  3 | Henry  |       2 |   23 | M    |    185 | 2015-05-31 |
  |  4 | Jane   |       1 |   22 | F    |    162 | 2016-12-20 |
  |  5 | Jim    |       1 |   24 | M    |    175 | 2016-01-15 |
  |  6 | John   |       2 |   21 | M    |    172 | 2015-11-11 |
  |  7 | Lily   |       6 |   22 | F    |    165 | 2016-02-26 |
  |  8 | Susan  |       4 |   23 | F    |    170 | 2015-10-01 |
  |  9 | Thomas |       3 |   22 | M    |    178 | 2016-06-07 |
  | 10 | Tom    |       4 |   23 | M    |    165 | 2016-08-05 |
  +----+--------+---------+------+------+--------+------------+
  #由执行结果可知，使用星号“*”通配符时，将返回所有列，数据列按照创建表时的顺序显示。 
  #注意：一般情况下，除非需要使用表中所有的字段数据，否则最好不要使用通配符“*”。使用通配符虽然可以节省输入查询语句的时间，但是获取不需要的列数据通常会降低查询和所使用的应用程序的效率。通配符的优势是，当不知道所需列的名称时，可以通过通配符获取它们。
  
  #eg2：
  mysql> SELECT id,name,dept_id,age,sex,height,login_date
      -> FROM tb_students_info;
  +----+--------+---------+------+------+--------+------------+
  | id | name   | dept_id | age  | sex  | height | login_date |
  +----+--------+---------+------+------+--------+------------+
  |  1 | Dany   |       1 |   25 | F    |    160 | 2015-09-10 |
  |  2 | Green  |       3 |   23 | F    |    158 | 2016-10-22 |
  |  3 | Henry  |       2 |   23 | M    |    185 | 2015-05-31 |
  |  4 | Jane   |       1 |   22 | F    |    162 | 2016-12-20 |
  |  5 | Jim    |       1 |   24 | M    |    175 | 2016-01-15 |
  |  6 | John   |       2 |   21 | M    |    172 | 2015-11-11 |
  |  7 | Lily   |       6 |   22 | F    |    165 | 2016-02-26 |
  |  8 | Susan  |       4 |   23 | F    |    170 | 2015-10-01 |
  |  9 | Thomas |       3 |   22 | M    |    178 | 2016-06-07 |
  | 10 | Tom    |       4 |   23 | M    |    165 | 2016-08-05 |
  +----+--------+---------+------+------+--------+------------+
  
  #查询表中指定字段：
  SELECT < 列名 > FROM < 表名 >；
  #eg3：mysql> SELECT name FROM tb_students_info;
  +--------+
  | name   |
  +--------+
  | Dany   |
  | Green  |
  | Henry  |
  | Jane   |
  | Jim    |
  | John   |
  | Lily   |
  | Susan  |
  | Thomas |
  | Tom    |
  +--------+
  
  #eg4：
  mysql> SELECT id,name,height
      -> FROM tb_students_info;
  +----+--------+--------+
  | id | name   | height |
  +----+--------+--------+
  |  1 | Dany   |    160 |
  |  2 | Green  |    158 |
  |  3 | Henry  |    185 |
  |  4 | Jane   |    162 |
  |  5 | Jim    |    175 |
  |  6 | John   |    172 |
  |  7 | Lily   |    165 |
  |  8 | Susan  |    170 |
  |  9 | Thomas |    178 |
  | 10 | Tom    |    165 |
  +----+--------+--------+
  
  ````



#### 17.去重[DISTINCT]

````mysql
SELECT DISTINCT <字段名> FROM <表名>;
#eg:
mysql> SELECT  DISTINCT age
    -> FROM tb_students_info;
+------+
| age  |
+------+
|   25 |
|   23 |
|   22 |
|   24 |
|   21 |
+------+
````



#### 18.设置别名[AS]

````mysql
#设置表别名
<表名> [AS] <别名>
#eg：
mysql> SELECT stu.name,stu.height
    -> FROM tb_students_info AS stu;
+--------+--------+
| name   | height |
+--------+--------+
| Dany   |    160 |
| Green  |    158 |
| Henry  |    185 |
| Jane   |    162 |
| Jim    |    175 |
| John   |    172 |
| Lily   |    165 |
| Susan  |    170 |
| Thomas |    178 |
| Tom    |    165 |
+--------+--------+

#设置列别名
<列名> [AS] <列别名>
#eg：
mysql> SELECT name AS student_name,
    -> age AS student_age
    -> FROM tb_students_info;
+--------------+-------------+
| student_name | student_age |
+--------------+-------------+
| Dany         |          25 |
| Green        |          23 |
| Henry        |          23 |
| Jane         |          22 |
| Jim          |          24 |
| John         |          21 |
| Lily         |          22 |
| Susan        |          23 |
| Thomas       |          22 |
| Tom          |          23 |
+--------------+-------------+
#注意：表别名只在执行查询时使用，并不在返回结果中显示，而列定义别名之后，将返回给客户端显示，显示的结果字段为字段列的别名。
````



#### 19.限制查询结果的记录条数[LIMIT]

SELECT 语句时往往返回的是所有匹配的行，有些时候我们仅需要返回第一行或者前几行，这时候就需要用到 MySQL LIMT 子句。

````mysql
<LIMIT> [<位置偏移量>,] <行数>
#eg1：显示结果前4行
mysql> SELECT * FROM tb_students_info LIMIT 4;
+----+-------+---------+------+------+--------+------------+
| id | name  | dept_id | age  | sex  | height | login_date |
+----+-------+---------+------+------+--------+------------+
|  1 | Dany  |       1 |   25 | F    |    160 | 2015-09-10 |
|  2 | Green |       3 |   23 | F    |    158 | 2016-10-22 |
|  3 | Henry |       2 |   23 | M    |    185 | 2015-05-31 |
|  4 | Jane  |       1 |   22 | F    |    162 | 2016-12-20 |
+----+-------+---------+------+------+--------+------------+

#eg2：返回从第 4 条记录开始的行数为 5 的记录
mysql> SELECT * FROM tb_students_info LIMIT 3,5;
+----+-------+---------+------+------+--------+------------+
| id | name  | dept_id | age  | sex  | height | login_date |
+----+-------+---------+------+------+--------+------------+
|  4 | Jane  |       1 |   22 | F    |    162 | 2016-12-20 |
|  5 | Jim   |       1 |   24 | M    |    175 | 2016-01-15 |
|  6 | John  |       2 |   21 | M    |    172 | 2015-11-11 |
|  7 | Lily  |       6 |   22 | F    |    165 | 2016-02-26 |
|  8 | Susan |       4 |   23 | F    |    170 | 2015-10-01 |
+----+-------+---------+------+------+--------+------------+
````



#### 20.对查询结果进行排序[ORDER BY]

````mysql
ORDER BY {<列名> | <表达式> | <位置>} [ASC|DESC]
/*语法说明如下。 
1) 列名
指定用于排序的列。可以指定多个列，列名之间用逗号分隔。 
2) 表达式
指定用于排序的表达式。 
3) 位置
指定用于排序的列在 SELECT 语句结果集中的位置，通常是一个正整数。 
4) ASC|DESC
关键字 ASC 表示按升序分组，关键字 DESC 表示按降序分组，其中 ASC 为默认值。这两个关键字必须位于对应的列名、表达式、列的位置之后。
*/

#eg1:查询 tb_students_info 表的 height 字段值，并对其进行排序
mysql> SELECT * FROM tb_students_info ORDER BY height;
+----+--------+---------+------+------+--------+------------+
| id | name   | dept_id | age  | sex  | height | login_date |
+----+--------+---------+------+------+--------+------------+
|  2 | Green  |       3 |   23 | F    |    158 | 2016-10-22 |
|  1 | Dany   |       1 |   25 | F    |    160 | 2015-09-10 |
|  4 | Jane   |       1 |   22 | F    |    162 | 2016-12-20 |
|  7 | Lily   |       6 |   22 | F    |    165 | 2016-02-26 |
| 10 | Tom    |       4 |   23 | M    |    165 | 2016-08-05 |
|  8 | Susan  |       4 |   23 | F    |    170 | 2015-10-01 |
|  6 | John   |       2 |   21 | M    |    172 | 2015-11-11 |
|  5 | Jim    |       1 |   24 | M    |    175 | 2016-01-15 |
|  9 | Thomas |       3 |   22 | M    |    178 | 2016-06-07 |
|  3 | Henry  |       2 |   23 | M    |    185 | 2015-05-31 |
+----+--------+---------+------+------+--------+------------+

#eg2:查询 tb_students_info 表中的 name 和 height 字段，先按 height 排序，再按 name 排序
mysql> SELECT name,height
    -> FROM tb_students_info
    -> ORDER BY height,name;
+--------+--------+
| name   | height |
+--------+--------+
| Green  |    158 |
| Dany   |    160 |
| Jane   |    162 |
| Lily   |    165 |
| Tom    |    165 |
| Susan  |    170 |
| John   |    172 |
| Jim    |    175 |
| Thomas |    178 |
| Henry  |    185 |
+--------+--------+
````



#### 21.条件查询[WHERE]

````mysql
WHERE <查询条件> {<判定运算1>，<判定运算2>，…}
/*
判定运算的语法分类如下：

- <表达式1>`{=|<|<=|>|>=|<=>|<>|！=}`<表达式2>
- <表达式1>`[NOT]LIKE`<表达式2>
- <表达式1>`[NOT][REGEXP|RLIKE]`<表达式2>
- <表达式1>`[NOT]BETWEEN`<表达式2>`AND`<表达式3>
- <表达式1>`IS[NOT]NULL`
*/

#eg1:[单条件]在表 tb_students_info 中查询身高为 170cm 的学生的姓名
mysql> use test_db
Database changed
mysql> SELECT name,height
    -> FROM tb_students_info
    -> WHERE height=170;
+-------+--------+
| name  | height |
+-------+--------+
| Susan |    170 |
+-------+--------+

#eg2：[多条件]在 tb_students_info 表中查询 age 大于 21，并且 height 大于等于 175 的学生的信息
mysql> SELECT * FROM tb_students_info
    -> WHERE age>21 AND height>=175;
+----+--------+---------+------+------+--------+------------+
| id | name   | dept_id | age  | sex  | height | login_date |
+----+--------+---------+------+------+--------+------------+
|  3 | Henry  |       2 |   23 | M    |    185 | 2015-05-31 |
|  5 | Jim    |       1 |   24 | M    |    175 | 2016-01-15 |
|  9 | Thomas |       3 |   22 | M    |    178 | 2016-06-07 |
+----+--------+---------+------+------+--------+------------+

#使用LIKE模糊查询
<表达式1> [NOT] LIKE <表达式2>
#通配符（注意：不要过度使用通配符，对通配符检索的处理一般会比其他检索方式花费更长的时间。）
/*
1) 百分号（%）
MySQL 默认是不区分大小写的，若要区分大小写，则需要更换字符集的校对规则。
百分号不匹配空值。
百分号可以代表搜索模式中给定位置的 0 个、1 个或多个字符。
尾空格可能会干扰通配符的匹配，一般可以在搜索模式的最后附加一个百分号。
2) 下划线（_）
下划线通配符和百分号通配符的用途一样，下画线只匹配单个字符，而不是多个字符，也不是 0 个字符。 
*/
#eg3：在 tb_students_info 表中，查找所有以字母“y”结尾，且“y”前面只有 4 个字母的学生的姓名
mysql> SELECT name FROM tb_students_info
    -> WHERE name LIKE '____y';
+-------+
| name  |
+-------+
| Henry |
+-------+

#日期字段作为条件的查询语句
#eg4：在表 tb_students_info 中查询注册日期在 2016-01-01 之前的学生的信息
mysql> SELECT * FROM tb_students_info
    -> WHERE login_date<'2016-01-01';
+----+-------+---------+------+------+--------+------------+
| id | name  | dept_id | age  | sex  | height | login_date |
+----+-------+---------+------+------+--------+------------+
|  1 | Dany  |       1 |   25 | F    |    160 | 2015-09-10 |
|  3 | Henry |       2 |   23 | M    |    185 | 2015-05-31 |
|  6 | John  |       2 |   21 | M    |    172 | 2015-11-11 |
|  8 | Susan |       4 |   23 | F    |    170 | 2015-10-01 |
+----+-------+---------+------+------+--------+------------+

#eg5：在表 tb_students_info 中查询注册日期在 2015-10-01 和 2016-05-01 之间的学生的信息
mysql> SELECT * FROM tb_students_info
    -> WHERE login_date
    -> BETWEEN '2015-10-01'
    -> AND '2016-05-01';
+----+-------+---------+------+------+--------+------------+
| id | name  | dept_id | age  | sex  | height | login_date |
+----+-------+---------+------+------+--------+------------+
|  5 | Jim   |       1 |   24 | M    |    175 | 2016-01-15 |
|  6 | John  |       2 |   21 | M    |    172 | 2015-11-11 |
|  7 | Lily  |       6 |   22 | F    |    165 | 2016-02-26 |
|  8 | Susan |       4 |   23 | F    |    170 | 2015-10-01 |
+----+-------+---------+------+------+--------+------------+
````



#### 22.内连接查询[INNER JOIN]

内连接是通过在查询中设置连接条件的方式，来移除查询结果集中某些数据行后的交叉连接。简单来说，就是利用条件表达式来消除交叉连接的某些数据行。

````mysql
SELECT <列名1，列名2 …>
FROM <表名1> INNER JOIN <表名2> [ ON子句]
#eg1:表 tb_students_info 和表 tb_departments 都包含相同数据类型的字段 dept_id，在两个表之间使用内连接查询
mysql> SELECT id,name,age,dept_name
    -> FROM tb_students_info,tb_departments
    -> WHERE tb_students_info.dept_id=tb_departments.dept_id;
+----+--------+------+-----------+
| id | name   | age  | dept_name |
+----+--------+------+-----------+
|  1 | Dany   |   25 | Computer  |
|  2 | Green  |   23 | Chinese   |
|  3 | Henry  |   23 | Math      |
|  4 | Jane   |   22 | Computer  |
|  5 | Jim    |   24 | Computer  |
|  6 | John   |   21 | Math      |
|  7 | Lily   |   22 | Computer  |
|  8 | Susan  |   23 | Economy   |
|  9 | Thomas |   22 | Chinese   |
| 10 | Tom    |   23 | Economy   |
+----+--------+------+-----------+


#eg2:使用 INNER JOIN 语法进行内连接查询
mysql> SELECT id,name,age,dept_name
    -> FROM tb_students_info INNER JOIN tb_departments
    -> WHERE tb_students_info.dept_id=tb_departments.dept_id;
+----+--------+------+-----------+
| id | name   | age  | dept_name |
+----+--------+------+-----------+
|  1 | Dany   |   25 | Computer  |
|  2 | Green  |   23 | Chinese   |
|  3 | Henry  |   23 | Math      |
|  4 | Jane   |   22 | Computer  |
|  5 | Jim    |   24 | Computer  |
|  6 | John   |   21 | Math      |
|  7 | Lily   |   22 | Computer  |
|  8 | Susan  |   23 | Economy   |
|  9 | Thomas |   22 | Chinese   |
| 10 | Tom    |   23 | Economy   |
+----+--------+------+-----------+

#使用 WHERE 子句定义连接条件比较简单明了，而 INNER JOIN 语法是 ANSI SQL 的标准规范，使用 INNER JOIN 连接语法能够确保不会忘记连接条件，而且 WHERE 子句在某些时候会影响查询的性能。
````



#### 23.外连接查询[OUTER JOIN]

外连接先将连接的表分为基表和参考表，再以基表为依据返回满足和不满足条件的记录。外连接更加注重两张表之间的关系。按照连接表的顺序，可以分为左外连接和右外连接。

````mysql
#在左外连接的结果集中，除了匹配的行之外，还包括左表中有但在右表中不匹配的行，对于这样的行，从右表中选择的列的值被设置为 NULL
#eg1：mysql> SELECT name,dept_name
    -> FROM tb_students_info s
    -> LEFT OUTER JOIN tb_departments d
    -> ON s.dept_id = d.dept_id;
+--------+-----------+
| name   | dept_name |
+--------+-----------+
| Dany   | Computer  |
| Jane   | Computer  |
| Jim    | Computer  |
| Henry  | Math      |
| John   | Math      |
| Green  | Chinese   |
| Thomas | Chinese   |
| Susan  | Economy   |
| Tom    | Economy   |
| Lily   | NULL      |
+--------+-----------+

#右外连接又称为右连接，在 FROM 子句中使用 RIGHT OUTER JOIN 或者 RIGHT JOIN。与左外连接相反，右外连接以右表为基表，连接方法和左外连接相同。在右外连接的结果集中，除了匹配的行外，还包括右表中有但在左表中不匹配的行，对于这样的行，从左表中选择的值被设置为 NULL。
#eg2：
mysql> SELECT name,dept_name
    -> FROM tb_students_info s
    -> RIGHT OUTER JOIN tb_departments d
    -> ON s.dept_id = d.dept_id;
+--------+-----------+
| name   | dept_name |
+--------+-----------+
| Dany   | Computer  |
| Green  | Chinese   |
| Henry  | Math      |
| Jane   | Computer  |
| Jim    | Computer  |
| John   | Math      |
| Susan  | Economy   |
| Thomas | Chinese   |
| Tom    | Economy   |
| NULL   | History   |
+--------+-----------+
````



#### 24.子查询[IN]

- 子查询指一个查询语句嵌套在另一个查询语句内部的查询，这个特性从 MySQL 4.1 开始引入，在 SELECT 子句中先计算子查询，子查询结果作为外层另一个查询的过滤条件，查询可以基于一个表或者多个表。

- 子查询中常用的操作符有 ANY（SOME）、ALL、IN 和 EXISTS。

- 子查询可以添加到 SELECT、UPDATE 和 DELETE 语句中，而且可以进行多层嵌套。子查询也可以使用比较运算符，如“<”、“<=”、“>”、“>=”、“！=”等。

````mysql
#in子查询
<表达式> [NOT] IN <子查询>
#比较运算符子查询
<表达式> {= | < | > | >= | <= | <=> | < > | != }
{ ALL | SOME | ANY} <子查询>
#exist子查询
EXIST <子查询>

#eg：在 tb_departments 表中查询 dept_type 为 A 的学院 ID，并根据学院 ID 查询该学院学生的名字
mysql> SELECT name FROM tb_students_info
    -> WHERE dept_id IN
    -> (SELECT dept_id
    -> FROM tb_departments
    -> WHERE dept_type= 'A' );
+-------+
| name  |
+-------+
| Dany  |
| Henry |
| Jane  |
| Jim   |
| John  |
+-------+
````



####  25.分组查询[GROUP BY]

- 在MYSQL SELECT 语句中，允许使用 GROUP BY 子句，将结果集中的数据行根据选择列的值进行逻辑分组，以便能汇总表内容的子集，实现对每个组而不是对整个结果集进行整合。

````mysql
GROUP BY { <列名> | <表达式> | <位置> } [ASC | DESC]
#eg：根据 dept_id 对 tb_students_info 表中的数据进行分组，将每个学院的学生姓名显示出来
mysql> SELECT dept_id,GROUP_CONCAT(name) AS names
    -> FROM tb_students_info
    -> GROUP BY dept_id;
+---------+---------------+
| dept_id | names         |
+---------+---------------+
|       1 | Dany,Jane,Jim |
|       2 | Henry,John    |
|       3 | Green,Thomas  |
|       4 | Susan,Tom     |
|       6 | Lily          |
+---------+---------------+
````



####  26.指定过滤条件[HAVING]

- 在MYSQL SELECT 语句中，除了能使用 GROUP BY 子句分组数据外，还可以使用 HAVING 子句过滤分组，在结果集中规定了包含哪些分组和排除哪些分组。

````mysql
HAVING <条件>
/*
HAVING 子句和 WHERE 子句非常相似，HAVING 子句支持 WHERE 子句中所有的操作符和语法，但是两者存在几点差异： 
WHERE 子句主要用于过滤数据行，而 HAVING 子句主要用于过滤分组，即 HAVING 子句基于分组的聚合值而不是特定行的值来过滤数据，主要用来过滤分组。
WHERE 子句不可以包含聚合函数，HAVING 子句中的条件可以包含聚合函数。
HAVING 子句是在数据分组后进行过滤，WHERE 子句会在数据分组前进行过滤。WHERE 子句排除的行不包含在分组中，可能会影响 HAVING 子句基于这些值过滤掉的分组。
*/
mysql> SELECT dept_id,GROUP_CONCAT(name) AS names
    -> FROM tb_students_info
    -> GROUP BY dept_id
    -> HAVING COUNT(name)>1;
+---------+---------------+
| dept_id | names         |
+---------+---------------+
|       1 | Dany,Jane,Jim |
|       2 | Henry,John    |
|       3 | Green,Thomas  |
|       4 | Susan,Tom     |
+---------+---------------+
````



#### 27.正则表达式查询[REGEXP]

| 选项          | 说明                                  | 例子                                        | 匹配值示例                  |
| ------------- | ------------------------------------- | ------------------------------------------- | --------------------------- |
| ^             | 匹配文本的开始字符                    | '^b' 匹配以字母 b 开头 的字符串             | book、big、banana、 bike    |
| $             | 匹配文本的结束字符                    | 'st$’ 匹配以 st 结尾的字 符串               | test、resist、persist       |
| .             | 匹配任何单个字符                      | 'b.t’ 匹配任何 b 和 t 之间有一个字符        | bit、bat、but、bite         |
| *             | 匹配零个或多个在它前面的字 符         | 'f*n’ 匹配字符 n 前面有 任意个字符 f        | fn、fan、faan、abcn         |
| +             | 匹配前面的字符 1 次或多次             | 'ba+’ 匹配以 b 开头，后 面至少紧跟一个 a    | ba、bay、bare、battle       |
| <字符串>      | 匹配包含指定字符的文本                | 'fa’                                        | fan、afa、faad              |
| [字符集合]    | 匹配字符集合中的任何一个字 符         | '[xz]'匹配 x 或者 z                         | dizzy、zebra、x-ray、 extra |
| [^]           | 匹配不在括号中的任何字符              | '[^abc]’ 匹配任何不包 含 a、b 或 c 的字符串 | desk、fox、f8ke             |
| 字符串{n,}    | 匹配前面的字符串至少 n 次             | b{2} 匹配 2 个或更多 的 b                   | bbb、 bbbb、 bbbbbbb        |
| 字符串  {n,m} | 匹配前面的字符串至少 n 次， 至多 m 次 | b{2,4} 匹配最少 2 个， 最多 4 个 b          | bbb、 bbbb                  |

````mysql
#eg:在 tb_departments 表中，查询 dept_name 字段以字母“C”开头的记录.
mysql> SELECT * FROM tb_departments
    -> WHERE dept_name REGEXP '^C';
+---------+-----------+-----------+-----------+
| dept_id | dept_name | dept_call | dept_type |
+---------+-----------+-----------+-----------+
|       1 | Computer  | 11111     | A         |
|       3 | Chinese   | 33333     | B         |
+---------+-----------+-----------+-----------+
````



#### 28.插入数据[INSERT INTO]

````mysql
#INSERT...VALUE
INSERT INTO <表名> [ <列名1> [ , … <列名n>] ]
VALUES (值1) [… , (值n) ];
#INSERT...SET
INSERT INTO <表名>
SET <列名1> = <值1>,
    <列名2> = <值2>,
    …
````

- 使用 INSERT…VALUES 语句可以向表中插入一行数据，也可以插入多行数据；
- 使用 INSERT…SET 语句可以指定插入行中每列的值，也可以指定部分列的值；
- INSERT…SELECT 语句向表中插入其他表的数据。
- 采用 INSERT…SET 语句可以向表中插入部分列的值，这种方式更为灵活；
- INSERT…VALUES 语句可以一次插入多条数据。

````mysql
#eg1：在 tb_courses 表中插入一条新记录，course_id 值为 1，course_name 值为“Network”，course_grade 值为 3，info 值为“Computer Network”。
mysql> INSERT INTO tb_courses
    -> (course_id,course_name,course_grade,course_info)
    -> VALUES(1,'Network',3,'Computer Network');
Query OK, 1 rows affected (0.08 sec)
mysql> SELECT * FROM tb_courses;
+-----------+-------------+--------------+------------------+
| course_id | course_name | course_grade | course_info      |
+-----------+-------------+--------------+------------------+
|         1 | Network     |            3 | Computer Network |
+-----------+-------------+--------------+------------------+

#eg2：从 tb_courses 表中查询所有的记录，并将其插入 tb_courses_new 表中。
mysql> INSERT INTO tb_courses_new
    -> (course_id,course_name,course_grade,course_info)
    -> SELECT course_id,course_name,course_grade,course_info
    -> FROM tb_courses;
Query OK, 4 rows affected (0.17 sec)
Records: 4  Duplicates: 0  Warnings: 0
mysql> SELECT * FROM tb_courses_new;
+-----------+-------------+--------------+------------------+
| course_id | course_name | course_grade | course_info      |
+-----------+-------------+--------------+------------------+
|         1 | Network     |            3 | Computer Network |
|         2 | Database    |            3 | MySQL            |
|         3 | Java        |            4 | Java EE          |
|         4 | System      |            3 | Operating System |
+-----------+-------------+--------------+------------------+
````



#### 29.修改数据[UPDATE]

````mysql
UPDATE <表名> SET 字段 1=值 1 [,字段 2=值 2… ] [WHERE 子句 ]
[ORDER BY 子句] [LIMIT 子句]
#eg1:在 tb_courses_new 表中，更新所有行的 course_grade 字段值为 4
mysql> UPDATE tb_courses_new
    -> SET course_grade=4;
Query OK, 3 rows affected (0.11 sec)
Rows matched: 4  Changed: 3  Warnings: 0
mysql> SELECT * FROM tb_courses_new;
+-----------+-------------+--------------+------------------+
| course_id | course_name | course_grade | course_info      |
+-----------+-------------+--------------+------------------+
|         1 | Network     |            4 | Computer Network |
|         2 | Database    |            4 | MySQL            |
|         3 | Java        |            4 | Java EE          |
|         4 | System      |            4 | Operating System |
+-----------+-------------+--------------+------------------+

#eg2:在 tb_courses 表中，更新 course_id 值为 2 的记录，将 course_grade 字段值改为 3.5，将 course_name 字段值改为“DB”
mysql> UPDATE tb_courses_new
    -> SET course_name='DB',course_grade=3.5
    -> WHERE course_id=2;
Query OK, 1 row affected (0.13 sec)
Rows matched: 1  Changed: 1  Warnings: 0
mysql> SELECT * FROM tb_courses_new;
+-----------+-------------+--------------+------------------+
| course_id | course_name | course_grade | course_info      |
+-----------+-------------+--------------+------------------+
|         1 | Network     |            4 | Computer Network |
|         2 | DB          |          3.5 | MySQL            |
|         3 | Java        |            4 | Java EE          |
|         4 | System      |            4 | Operating System |
+-----------+-------------+--------------+------------------+
````



#### 30.删除数据[DELETE FROM]

````mysql
DELETE FROM <表名> [WHERE 子句] [ORDER BY 子句] [LIMIT 子句]
/*
<表名>：指定要删除数据的表名。
ORDER BY 子句：可选项。表示删除时，表中各行将按照子句中指定的顺序进行删除。
WHERE 子句：可选项。表示为删除操作限定删除条件，若省略该子句，则代表删除该表中的所有行。
LIMIT 子句：可选项。用于告知服务器在控制命令被返回到客户端前被删除行的最大值。
*/
#eg:在 tb_courses_new 表中，删除 course_id 为 4 的记录
mysql> DELETE FROM tb_courses
    -> WHERE course_id=4;
Query OK, 1 row affected (0.00 sec)
mysql> SELECT * FROM tb_courses;
+-----------+-------------+--------------+------------------+
| course_id | course_name | course_grade | course_info      |
+-----------+-------------+--------------+------------------+
|         1 | Network     |            3 | Computer Network |
|         2 | Database    |            3 | MySQL            |
|         3 | Java        |            4 | Java EE          |
+-----------+-------------+--------------+------------------+
````



#### 31.视图[VIEW]

视图是一个虚拟表，其内容由查询定义。同真实表一样，视图包含一系列带有名称的列和行数据，但视图并不是数据库真实存储的数据表。

 视图是从一个、多个表或者视图中导出的表，包含一系列带有名称的数据列和若干条数据行。

 视图并不同于数据表，它们的区别在于以下几点：

- 视图不是数据库中真实的表，而是一张虚拟表，其结构和数据是建立在对数据中真实表的查询基础上的。
- 存储在数据库中的查询操作 SQL 语句定义了视图的内容，列数据和行数据来自于视图查询所引用的实际表，引用视图时动态生成这些数据。
- 视图没有实际的物理记录，不是以数据集的形式存储在数据库中的，它所对应的数据实际上是存储在视图所引用的真实表中的。
- 视图是数据的窗口，而表是内容。表是实际数据的存放单位，而视图只是以不同的显示方式展示数据，其数据来源还是实际表。
- 视图是查看数据表的一种方法，可以查询数据表中某些字段构成的数据，只是一些 SQL 语句的集合。从安全的角度来看，视图的数据安全性更高，使用视图的用户不接触数据表，不知道表结构。
- 视图的建立和删除只影响视图本身，不影响对应的基本表。



````mysql
#创建视图
CREATE VIEW <视图名> AS <SELECT语句>
#eg1:创建基于单表的视图
mysql> CREATE VIEW view_students_info
    -> AS SELECT * FROM tb_students_info;
Query OK, 0 rows affected (0.00 sec)
mysql> SELECT * FROM view_students_info;
+----+--------+---------+------+------+--------+------------+
| id | name   | dept_id | age  | sex  | height | login_date |
+----+--------+---------+------+------+--------+------------+
|  1 | Dany   |       1 |   25 | F    |    160 | 2015-09-10 |
|  2 | Green  |       3 |   23 | F    |    158 | 2016-10-22 |
|  3 | Henry  |       2 |   23 | M    |    185 | 2015-05-31 |
|  4 | Jane   |       1 |   22 | F    |    162 | 2016-12-20 |
|  5 | Jim    |       1 |   24 | M    |    175 | 2016-01-15 |
|  6 | John   |       2 |   21 | M    |    172 | 2015-11-11 |
|  7 | Lily   |       6 |   22 | F    |    165 | 2016-02-26 |
|  8 | Susan  |       4 |   23 | F    |    170 | 2015-10-01 |
|  9 | Thomas |       3 |   22 | M    |    178 | 2016-06-07 |
| 10 | Tom    |       4 |   23 | M    |    165 | 2016-08-05 |
+----+--------+---------+------+------+--------+------------+

#eg2:创建基于多表的视图
````



````mysql
#修改视图
ALTER VIEW <视图名> AS <SELECT语句>
#注意：对视图的修改就是对基本表的修改，因此在修改时，要满足基本表的数据定义。
````

某些视图是可更新的。也就是说，可以使用 UPDATE、DELETE 或 INSERT 等语句更新基本表的内容。对于可更新的视图，视图中的行和基本表的行之间必须具有一对一的关系。

还有一些特定的其他结构，这些结构会使得视图不可更新。更具体地讲，如果视图包含以下结构中的任何一种，它就是不可更新的：

- 聚合函数 SUM()、MIN()、MAX()、COUNT() 等。
- DISTINCT 关键字。
- GROUP BY 子句。
- HAVING 子句。
- UNION 或 UNION ALL 运算符。
- 位于选择列表中的子查询。
- FROM 子句中的不可更新视图或包含多个表。
- WHERE 子句中的子查询，引用 FROM 子句中的表。
- ALGORITHM 选项为 TEMPTABLE（使用临时表总会使视图成为不可更新的）的时候。



````mysql
#删除视图
DROP VIEW <视图名1> [ , <视图名2> …]
#eg:
mysql> DROP VIEW IF EXISTS v_students_info;
````



#### 32.自定义函数[CREATE FUNCTION]

自定义函数是一种与存储过程十分相似的过程式数据库对象。它与存储过程一样，都是由 SQL 语句和过程式语句组成的代码片段，并且可以被应用程序和其他 SQL 语句调用。

 自定义函数与存储过程之间存在几点区别：

- 自定义函数不能拥有输出参数，这是因为自定义函数自身就是输出参数；而存储过程可以拥有输出参数。
- 自定义函数中必须包含一条 RETURN 语句，而这条特殊的 SQL 语句不允许包含于存储过程中。
- 可以直接对自定义函数进行调用而不需要使用 CALL 语句，而对存储过程的调用需要使用 CALL 语句。3

````mysql
##创建自定义函数
CREATE FUNCTION <函数名> ( [ <参数1> <类型1> [ , <参数2> <类型2>] ] … )
  RETURNS <类型>
  <函数主体>

#eg1:创建存储函数，名称为 StuNameById，该函数返回 SELECT 语句的查询结果，数值类型为字符串类型
mysql> CREATE FUNCTION StuNameById()
    -> RETURNS VARCHAR(45)
    -> RETURN
    -> (SELECT name FROM tb_students_info
    -> WHERE id=1);
    
#修改自定义函数
#可以使用 ALTER FUNCTION 语句来修改自定义函数的某些相关特征。若要修改自定义函数的内容，则需要先删除该自定义函数，然后重新创建。 

#删除自定义函数
DROP FUNCTION [ IF EXISTS ] <自定义函数名>
````



#### 33.存储过程[PROCEDURE]

- 存储过程是一组为了完成特定功能的 SQL 语句集合。使用存储过程的目的是将常用或复杂的工作预先用 SQL 语句写好并用一个指定名称存储起来，这个过程经编译和优化后存储在数据库服务器中，因此称为存储过程。当以后需要数据库提供与已定义好的存储过程的功能相同的服务时，只需调用“CALL存储过程名字”即可自动完成。
- 一个存储过程是一个可编程的函数，它在数据库中创建并保存，一般由 SQL 语句和一些特殊的控制结构组成。当希望在不同的应用程序或平台上执行相同的特定功能时，存储过程尤为合适。
- 存储过程通常有如下优点：
  1. 封装性：存储过程被创建后，可以在程序中被多次调用，而不必重新编写该存储过程的 SQL 语句，并且数据库专业人员可以随时对存储过程进行修改，而不会影响到调用它的应用程序源代码。
  2. 可增强SQL语句的功能和灵活性：存储过程可以用流程控制语句编写，有很强的灵活性，可以完成复杂的判断和较复杂的运算。
  3. 可减少网络流量：由于存储过程是在服务器端运行的，且执行速度快，因此当客户计算机上调用该存储过程时，网络中传送的只是该调用语句，从而可降低网络负载。
  4. 高性能：存储过程执行一次后，产生的二进制代码就驻留在缓冲区，在以后的调用中，只需要从缓冲区中执行二进制代码即可，从而提高了系统的效率和性能。
  5. 提高数据库的安全性和数据的完整性：使用存储过程可以完成所有数据库操作，并且可以通过编程的方式控制数据库信息访问的权限。

````mysql
#创建存储过程
CREATE PROCEDURE <过程名> ( [过程参数[,…] ] ) <过程体>
[过程参数[,…] ] 格式
[ IN | OUT | INOUT ] <参数名> <类型>
````

[语法说明](http://c.biancheng.net/view/2593.html)

````mysql
#创建不带参数的存储过程
#eg1：创建名称为 ShowStuScore 的存储过程，存储过程的作用是从学生成绩信息表中查询学生的成绩信息
mysql> DELIMITER //
mysql> CREATE PROCEDURE ShowStuScore()
    -> BEGIN
    -> SELECT * FROM tb_students_score;
    -> END //
#创建完成后调用
mysql> DELIMITER ;
mysql> CALL ShowStuScore();
+--------------+---------------+
| student_name | student_score |
+--------------+---------------+
| Dany         |            90 |
| Green        |            99 |
| Henry        |            95 |
| Jane         |            98 |
| Jim          |            88 |
| John         |            94 |
| Lily         |           100 |
| Susan        |            96 |
| Thomas       |            93 |
| Tom          |            89 |
+--------------+---------------+

#创建带参数的存储过程
#eg2：创建名称为 GetScoreByStu 的存储过程，输入参数是学生姓名。存储过程的作用是通过输入的学生姓名从学生成绩信息表中查询指定学生的成绩信息
mysql> DELIMITER //
mysql> CREATE PROCEDURE GetScoreByStu
    -> (IN name VARCHAR(30))
    -> BEGIN
    -> SELECT student_score FROM tb_students_score
    -> WHERE student_name=name;
    -> END //
#创建完成后调用
mysql> DELIMITER ;
mysql> CALL GetScoreByStu('Green');
+---------------+
| student_score |
+---------------+
|            99 |
+---------------+
````

````mysql
#修改存储过程
ALTER PROCEDURE 存储过程名 [ 特征 ... ]
#eg：下面修改存储过程 showstuscore 的定义，将读写权限改为 MODIFIES SQL DATA，并指明调用者可以执行
mysql> ALTER PROCEDURE showstuscore MODIFIES SQL DATA SQL SECURITY INVOKER;

#ALTER PROCEDURE 语句用于修改存储过程的某些特征。如果要修改存储过程的内容，可以先删除原存储过程，再以相同的命名创建新的存储过程；如果要修改存储过程的名称，可以先删除原存储过程，再以不同的命名创建新的存储过程。

#删除存储过程
DROP { PROCEDURE | FUNCTION } [ IF EXISTS ] <过程名>
#eg：
mysql> DROP PROCEDURE showstuscore;
````



#### 34.触发器[TRIGGER]

触发器是一个特殊的存储过程，不同的是执行存储过程要使用 CALL 语句来调用，而触发器的执行不需要使用 CALL 语句来调用，也不需要手工启动，只要一个预定义的事件发生就会被 MySQL自动调用。

引发触发器执行的事件一般如下：

- 增加一条学生记录时，会自动检查年龄是否符合范围要求。
- 每当删除一条学生信息时，自动删除其成绩表上的对应记录。
- 每当删除一条数据时，在数据库存档表中保留一个备份副本。


 触发程序的优点如下：

- 触发程序的执行是自动的，当对触发程序相关表的数据做出相应的修改后立即执行。
- 触发程序可以通过数据库中相关的表层叠修改另外的表。
- 触发程序可以实施比 FOREIGN KEY 约束、CHECK 约束更为复杂的检查和操作。


 触发器与表关系密切，主要用于保护表中的数据。特别是当有多个表具有一定的相互联系的时候，触发器能够让不同的表保持数据的一致性。

 在 MySQL 中，只有执行 INSERT、UPDATE 和 DELETE 操作时才能激活触发器。

 在实际使用中，MySQL 所支持的触发器有三种：INSERT 触发器、UPDATE 触发器和 DELETE 触发器。

* INSERT触发器：在INSERT语句执行之前或之后响应的触发器

  > 在insert触发器代码内，可引用一个名为new的虚拟表来访问被插入的行
  >
  > 在before insert触发器中，new中的值也可以被更新，即允许更改被插入的值
  >
  > 对于auto_increment列，new在insert执行之前包含的值是0，在insert执行之后将包含新的自动生成值

* UPDATE触发器：在UPDATE语句执行之前或之后响应的触发器

  > 在 UPDATE 触发器代码内，可引用一个名为 NEW（不区分大小写）的虚拟表来访问更新的值。
  >
  > 在 UPDATE 触发器代码内，可引用一个名为 OLD（不区分大小写）的虚拟表来访问 UPDATE 语句执行前的值。
  >
  > 在 BEFORE UPDATE 触发器中，NEW 中的值可能也被更新，即允许更改将要用于 UPDATE 语句中的值（只要具有对应的操作权限）。
  >
  > OLD 中的值全部是只读的，不能被更新。

* DELETE触发器：在DELETE语句执行之前或之后响应的触发器

  > 在 DELETE 触发器代码内，可以引用一个名为 OLD（不区分大小写）的虚拟表来访问被删除的行。
  >
  > OLD 中的值全部是只读的，不能被更新。



````mysql
#创建触发器
CREATE <触发器名> < BEFORE | AFTER >
<INSERT | UPDATE | DELETE >
ON <表名> FOR EACH Row<触发器主体>

#eg1：创建一个名为 SumOfSalary 的触发器，触发的条件是向数据表 tb_emp8 中插入数据之前，对新插入的 salary 字段值进行求和计算
mysql> CREATE TRIGGER SumOfSalary
    -> BEFORE INSERT ON tb_emp8
    -> FOR EACH ROW
    -> SET @sum=@sum+NEW.salary;
    
#eg2：创建一个名为 double_salary 的触发器，触发的条件是向数据表 tb_emp6 中插入数据之后，再向数据表 tb_emp7 中插入相同的数据，并且 salary 为 tb_emp6 中新插入的 salary 字段值的 2 倍
mysql> CREATE TRIGGER double_salary
    -> AFTER INSERT ON tb_emp6
    -> FOR EACH ROW
    -> INSERT INTO tb_emp7
    -> VALUES (NEW.id,NEW.name,deptId,2*NEW.salary);
    
#删除触发器
DROP TRIGGER [ IF EXISTS ] [数据库名] <触发器名>
#执行DROP TRIGGER需要SUPER权限
#eg：mysql> DROP TRIGGER double_salary;
````



#### 35.索引[INDEX]

* 访问数据库表行数据的两种方式

  顺序访问：从到到尾逐行遍历，直到在无序的行数据中找到符合条件的目标数据。效率低性能差。

  索引访问：通过遍历索引来直接访问表中记录行的方式。索引存储了指定列数据值的指针，根据指定的排序顺序对这些指针排序。

* 索引分类

  根据存储方式不同：B-树索引、哈希索引、

  根据具体用途：普通索引、唯一性索引、主键索引、空间索引、全文索引

  索引在逻辑上分为以上 5 类，但在实际使用中，索引通常被创建成单列索引和组合索引。

  > 单列索引就是索引只包含原表的一个列。
  >
  > 组合索引也称为复合索引或多列索引，相对于单列索引来说，组合索引是将原表的多个列共同组成一个索引。

* 建立索引的原则
  1. 在经常需要搜索的列上建立索引，可以加快搜索的速度。
  2. 在作为主键的列上创建索引，强制该列的唯一性，并组织表中数据的排列结构。
  3. 在经常使用表连接的列上创建索引，这些列主要是一些外键，可以加快表连接的速度。
  4. 在经常需要根据范围进行搜索的列上创建索引，因为索引已经排序，所以其指定的范围是连续的。
  5. 在经常需要排序的列上创建索引，因为索引已经排序，所以查询时可以利用索引的排序，加快排序查询。
  6. 在经常使用 WHERE 子句的列上创建索引，加快条件的判断速度。

* 创建索引

  ````mysql
  #CREATE INDEX
  CREATE <索引名> ON <表名> (<列名> [<长度>] [ ASC | DESC])
  
  #CREATE TABLE
  #在创建表时同时创建
  CONSTRAINT PRIMARY KEY [索引类型] (<列名>,…)
  KEY | INDEX [<索引名>] [<索引类型>] (<列名>,…)
  UNIQUE [ INDEX | KEY] [<索引名>] [<索引类型>] (<列名>,…)
  FOREIGN KEY <索引名> <列名>
  
  #ALTER TABLE
  #在已创建的表上添加索引
  ADD INDEX [<索引名>] [<索引类型>] (<列名>,…)
  ADD PRIMARY KEY [<索引类型>] (<列名>,…)
  ADD UNIQUE [ INDEX | KEY] [<索引名>] [<索引类型>] (<列名>,…)
  ADD FOREIGN KEY [<索引名>] (<列名>,…)
  
  #eg1：创建一个表 tb_stu_info，在该表的 height 字段创建一般索引。
  mysql> CREATE TABLE tb_stu_info
      -> (
      -> id INT NOT NULL,
      -> name CHAR(45) DEFAULT NULL,
      -> dept_id INT DEFAULT NULL,
      -> age INT DEFAULT NULL,
      -> height INT DEFAULT NULL,
      -> INDEX(height)
      -> );
      
  #eg2：创建一个表 tb_stu_info2，在该表的 id 字段上使用 UNIQUE 关键字创建唯一索引
  mysql> CREATE TABLE tb_stu_info2
      -> (
      -> id INT NOT NULL,
      -> name CHAR(45) DEFAULT NULL,
      -> dept_id INT DEFAULT NULL,
      -> age INT DEFAULT NULL,
      -> height INT DEFAULT NULL,
      -> UNIQUE INDEX(height)
      -> );
  ````

* 查看索引

  ````mysql
  SHOW INDEX FROM <表名> [ FROM <数据库名>]
  #eg：
  mysql> SHOW INDEX FROM tb_stu_info2\G
  *************************** 1. row ***************************
          Table: tb_stu_info2
     Non_unique: 0
       Key_name: height
  Seq_in_index: 1
    Column_name: height
      Collation: A
    Cardinality: 0
       Sub_part: NULL
         Packed: NULL
           Null: YES
     Index_type: BTREE
        Comment:
  Index_comment:
  ````

* 修改和删除索引

  ````mysql
  #DROP INDEX
  DROP INDEX <索引名> ON <表名>
  
  #ALTER TABLE
  /*
  根据 ALTER TABLE 语句的语法可知，该语句也可以用于删除索引。具体使用方法是将 ALTER TABLE 语句的语法中部分指定为以下子句中的某一项。
      DROP PRIMARY KEY：表示删除表中的主键。一个表只有一个主键，主键也是一个索引。
      DROP INDEX index_name：表示删除名称为 index_name 的索引。
      DROP FOREIGN KEY fk_symbol：表示删除外键。
  */
  
  #eg1：删除表 tb_stu_info 中的索引
  mysql> DROP INDEX height
      -> ON tb_stu_info;
  #eg2：删除表 tb_stu_info2 中名称为 id 的索引
  mysql> ALTER TABLE tb_stu_info2
      -> DROP INDEX height;
  ````

  

#### 36.用户[USER]

* 创建用户

  ````mysql
  CREATE USER <用户名> [ IDENTIFIED ] BY [ PASSWORD ] <口令>
  #eg:使用 CREATE USER 创建一个用户，用户名是 james，密码是 tiger，主机是 localhost
  mysql> CREATE USER 'james'@'localhost'
      -> IDENTIFIED BY 'tiger';
  ````

* 修改用户

  ````mysql
  #修改用户名
  RENAME USER <旧用户> TO <新用户>
  
  #修改用户口令
  SET PASSWORD [ FOR <用户名> ] =
  {
      PASSWORD('新明文口令')
      | OLD_PASSWORD('旧明文口令')
      | '加密口令值'
  }
  #eg：
  mysql> SET PASSWORD FOR 'jack'@'localhost'=
      -> PASSWORD('lion');
  ````

* 删除用户

  ````mysql
  DROP USER <用户名1> [ , <用户名2> ]…
  #eg:
  mysql> DROP USER 'jack'@'localhost';
  ````

* 用户权限

  ````mysql
  GRANT
  <权限类型> [ ( <列名> ) ] [ , <权限类型> [ ( <列名> ) ] ]
  ON <对象> <权限级别> TO <用户>
  其中<用户>的格式：
  <用户名> [ IDENTIFIED ] BY [ PASSWORD ] <口令>
  [ WITH GRANT OPTION]
  | MAX_QUERIES_PER_HOUR <次数>
  | MAX_UPDATES_PER_HOUR <次数>
  | MAX_CONNECTIONS_PER_HOUR <次数>
  | MAX_USER_CONNECTIONS <次数>
  ````

  用于指定权限的级别。可以授予的权限有如下几组：

  > 1. 列权限，和表中的一个具体列相关。例如，可以使用 UPDATE 语句更新表 students 中 student_name 列的值的权限。
  >
  >    ```
  >    授予列权限时，<权限类型>的值只能指定为 SELECT、INSERT 和 UPDATE，同时权限的后面需要加上列名列表 column-list。
  >    ```
  >
  > 2. 表权限，和一个具体表中的所有数据相关。例如，可以使用 SELECT 语句查询表 students 的所有数据的权限。
  >
  >    ```
  >    - SELECT：授予用户可以使用 SELECT 语句进行访问特定表的权限。
  >    - INSERT：授予用户可以使用 INSERT 语句向一个特定表中添加数据行的权限。
  >    - DELETE：授予用户可以使用 DELETE 语句从一个特定表中删除数据行的权限。
  >    - DROP：授予用户可以删除数据表的权限。
  >    - UPDATE：授予用户可以使用 UPDATE 语句更新特定数据表的权限。
  >    - ALTER：授予用户可以使用 ALTER TABLE 语句修改数据表的权限。
  >    - REFERENCES：授予用户可以创建一个外键来参照特定数据表的权限。
  >    - CREATE：授予用户可以使用特定的名字创建一个数据表的权限。
  >    - INDEX：授予用户可以在表上定义索引的权限。
  >    - ALL 或 ALL PRIVILEGES：所有的权限名。
  >    ```
  >
  >    
  >
  > 3. 数据库权限，和一个具体的数据库中的所有表相关。例如，可以在已有的数据库 mytest 中创建新表的权限。
  >
  >    ```
  >    - SELECT：表示授予用户可以使用 SELECT 语句访问特定数据库中所有表和视图的权限。
  >    - INSERT：表示授予用户可以使用 INSERT 语句向特定数据库中所有表添加数据行的权限。
  >    - DELETE：表示授予用户可以使用 DELETE 语句删除特定数据库中所有表的数据行的权限。
  >    - UPDATE：表示授予用户可以使用 UPDATE 语句更新特定数据库中所有数据表的值的权限。
  >    - REFERENCES：表示授予用户可以创建指向特定的数据库中的表外键的权限。
  >    - CREATE：表示授权用户可以使用 CREATE TABLE 语句在特定数据库中创建新表的权限。
  >    - ALTER：表示授予用户可以使用 ALTER TABLE 语句修改特定数据库中所有数据表的权限。
  >    - SHOW VIEW：表示授予用户可以查看特定数据库中已有视图的视图定义的权限。
  >    - CREATE ROUTINE：表示授予用户可以为特定的数据库创建存储过程和存储函数的权限。
  >    - ALTER ROUTINE：表示授予用户可以更新和删除数据库中已有的存储过程和存储函数的权限。
  >    - INDEX：表示授予用户可以在特定数据库中的所有数据表上定义和删除索引的权限。
  >    - DROP：表示授予用户可以删除特定数据库中所有表和视图的权限。
  >    - CREATE TEMPORARY TABLES：表示授予用户可以在特定数据库中创建临时表的权限。
  >    - CREATE VIEW：表示授予用户可以在特定数据库中创建新的视图的权限。
  >    - EXECUTE ROUTINE：表示授予用户可以调用特定数据库的存储过程和存储函数的权限。
  >    - LOCK TABLES：表示授予用户可以锁定特定数据库的已有数据表的权限。
  >    - ALL 或 ALL PRIVILEGES：表示以上所有权限。
  >    ```
  >
  >    
  >
  > 4. 用户权限，和 MySQL 中所有的数据库相关。例如，可以删除已有的数据库或者创建一个新的数据库的权限。
  >
  >    ```
  >    - CREATE USER：表示授予用户可以创建和删除新用户的权限。
  >    - SHOW DATABASES：表示授予用户可以使用 SHOW DATABASES 语句查看所有已有的数据库的定义的权限。
  >    ```
  >
  >    

  对应地，在 GRANT 语句中可用于指定权限级别的值有以下几类格式：

  > 1. *：表示当前数据库中的所有表。
  > 2. *.*：表示所有数据库中的所有表。
  > 3. db_name.*：表示某个数据库中的所有表，db_name 指定数据库名。
  > 4. db_name.tbl_name：表示某个数据库中的某个表或视图，db_name 指定数据库名，tbl_name 指定表名或视图名。
  > 5. tbl_name：表示某个表或视图，tbl_name 指定表名或视图名。
  > 6. db_name.routine_name：表示某个数据库中的某个存储过程或函数，routine_name 指定存储过程名或函数名。
  > 7. TO 子句：用来设定用户口令，以及指定被赋予权限的用户 user。若在 TO  子句中给系统中存在的用户指定口令，则新密码会将原密码覆盖；如果权限被授予给一个不存在的用户，MySQL 会自动执行一条 CREATE USER  语句来创建这个用户，但同时必须为该用户指定口令。

  ````mysql
  #eg:使用 GRANT 语句创建一个新的用户 testUser，密码为 testPwd。用户 testUser 对所有的数据有查询、插入权限，并授予 GRANT 权限。
  mysql> GRANT SELECT,INSERT ON *.*
      -> TO 'testUser'@'localhost'
      -> IDENTIFIED BY 'testPwd'
      -> WITH GRANT OPTION;
  ````

* 删除用户权限

  ````mysql
  #first
  REVOKE <权限类型> [ ( <列名> ) ] [ , <权限类型> [ ( <列名> ) ] ]…
  ON <对象类型> <权限名> FROM <用户1> [ , <用户2> ]…
  
  #second
  REVOKE ALL PRIVILEGES, GRANT OPTION
  FROM user <用户1> [ , <用户2> ]…
  
  #eg：使用 REVOKE 语句取消用户 testUser 的插入权限
  mysql> REVOKE INSERT ON *.*
      -> FROM 'testUser'@'localhost';
  mysql> SELECT Host,User,Select_priv,Insert_priv,Grant_priv
      -> FROM mysql.user
      -> WHERE User='testUser';
  +-----------+----------+-------------+-------------+------------+
  | Host      | User     | Select_priv | Insert_priv | Grant_priv |
  +-----------+----------+-------------+-------------+------------+
  | localhost | testUser | Y           | N           | Y          |
  +-----------+----------+-------------+-------------+------------+
  ````



#### 37.事务[TRANSACTION]

* 事务的四个特征

  原子性、一致性、隔离性、持续性

* 开始事务

  ````mysql
  BEGIN TRANSACTION <事务名称> |@<事务变量名称>
  #@<事务变量名称>是由用户定义的变量，必须用 char、varchar、nchar 或 nvarchar数据类型来声明该变量。
  #BEGIN TRANSACTION 语句的执行使全局变量 @@TRANCOUNT 的值加 1。
  ````

* 提交事务

  ````mysql
  COMMIT TRANSACTION <事务名称> |@<事务变量名称>
  #提交事务，意味着将事务开始以来所执行的所有数据修改成为数据库的永久部分，因此也标志着一个事务的结束。一旦执行了该命令，将不能回滚事务。只有在所有修改都准备好提交给数据库时，才执行这一操作。
  ````

* 撤销事务

  ````mysql
  ROLLBACK [TRANSACTION]
  [<事务名称>| @<事务变量名称> | <存储点名称>| @ <含有存储点名称的变量名>
  #当事务执行过程中遇到错误时，使用 ROLLBACK TRANSACTION 语句使事务回滚到起点或指定的保持点处。同时，系统将清除自事务起点或到某个保存点所做的所有的数据修改，并且释放由事务控制的资源。因此，这条语句也标志着事务的结束。
   
  #当条件回滚只影响事务的一部分时，事务不需要全部撤销已执行的操作。可以让事务回滚到指定位置，此时，需要在事务中设定保存点（SAVEPOINT）。保存点所在位置之前的事务语句不用回滚，即保存点之前的操作被视为有效的。保存点的创建通过“SAVING TRANSACTION<保存点名称>”语句来实现，再执行“ROLLBACK TRANSACTION<保存点名称>”语句回滚到该保存点。
  
  #若事务回滚到起点，则全局变量 @@TRANCOUNT 的值减 1；若事务回滚到指定的保存点，则全局变量 @@TRANCOUNT 的值不变。
  ````



#### 38.数据库备份[SELECT INTO OUTFILE]

* 数据库备份是指通过导出数据或者复制表文件的方式来制作数据库的副本。当数据库出现故障或遭到破坏时，将备份的数据库加载到系统，从而使数据库从错误状态恢复到备份时的正确状态。

* 可以使用 SELECT INTO OUTFILE 语句把表数据导出到一个文本文件中进行备份。但这种方法只能导出或导入数据的内容，而不包括表的结构。若表的结构文件损坏，则必须先设法恢复原来表的结构。

  ````mysql
  #eg:将数据库 test_db 的表 tb_students_info 的全部数据备份到 C 盘的数据备份目录下文件名为 file.txt 的文件中，要求每个字段用逗号分开，并且字符用双引号标注，每行以问号结束。
  mysql> SELECT * FROM test_db.tb_students_info
      -> INTO OUTFILE 'C:/ProgramData/MySQL/MySQL Server 5.7/Uploads/file.txt'
      -> FIELDS TERMINATED BY '"'
      -> LINES TERMINATED BY '?';
  ````



#### 39.数据库恢复

- 系统进行恢复操作时，先执行一些系统安全性的检查，包括检查所要恢复的数据库是否存在、数据库是否变化及数据库文件是否兼容等，然后根据所采用的数据库备份类型采取相应的恢复措施。

-  数据库恢复机制设计的两个关键问题是：第一，如何建立冗余数据；第二，如何利用这些冗余数据实施数据库恢复。

-  建立冗余数据最常用的技术是数据转储和登录日志文件。通常在一个数据库系统中，这两种方法是一起使用的。

-  数据转储是 DBA 定期地将整个数据库复制到磁带或另一个磁盘上保存起来的过程。这些备用的版本成为后备副本或后援副本。

-  可使用 LOAD DATA…INFILE 语句来恢复先前备份的数据。

````mysql
#eg:将之前导出的数据备份文件 file.txt 导入数据库 test_db 的表 tb_students_copy 中，其中 tb_students_copy 的表结构和 tb_students_info 相同。
mysql> CREATE TABLE tb_students_copy
    -> LIKE tb_students_info;
mysql> LOAD DATA INFILE 'C:/ProgramData/MySQL/MySQL Server 5.7/
Uploads/file.txt'
    -> INTO TABLE test_db.tb_students_copy
    -> FIELDS TERMINATED BY ','
    -> OPTIONALLY ENCLOSED BY '"'
    -> LINES TERMINATED BY '?';
````

