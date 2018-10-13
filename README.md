+ 练习环境
使用xampp傻瓜式安装包，打开xampp control panel，启动apache和mysql，打开phpadmin

+ 创建数据库

  `create database 数据库名`

+ 删除数据库

  `drop database 数据库名`

+ 创建数据表
    - 表名
    - 表字段名
    - 定义每个表字段
    
```
  CREATE TABLE IF NOT EXISTS `runoob_tbl`(
    `runoob_id` INT UNSIGNED AUTO_INCREMENT,
    `runoob_title` VARCHAR(100) NOT NULL,
    `runoob_author` VARCHAR(40) NOT NULL,
    `submission_date` DATE,
    PRIMARY KEY ( `runoob_id` )
    )ENGINE=InnoDB DEFAULT CHARSET=utf8;
```
　
    1. 设置表的非空约束

　　简单的说就是不让这个属性的值为空，不填的话就会报错

　　`格式：表字段名 数据类型 NOT NULL`

 
　　2. 设置表的唯一性约束

　　就是这个属性的值是不能重复的

　　`格式：表字段名 数据类型 UNIQUE`

 
　　3. 设置表的属性值自动增加

　　AUTO_INCREMENT约束的字段可以是任何整数类型（TINYINT、SMALLINT、INT和BIGINT），在默认的情况下，该字段的值是从1开始自增

　　`格式：表字段名 数据类型 AUTO_INCREMENT`

 
　　4. 设置表的属性的默认值

　　`格式：表字段名 数据类型 DEFAULT 默认值`
