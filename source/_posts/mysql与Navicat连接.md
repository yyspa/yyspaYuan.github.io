---
title: mysql与Navicat连接
categories: MySQL
tags: 
  - 问题
  - MySQL
---

# [解决：navicat出现Table ‘performance_schema.session_variables’ doesn’t exist报错，解决过程中出现mysql遇到的cannot select database 问题](https://www.cnblogs.com/hellowen/p/12967726.html)

问题描述：

navicat连接本地MySQL时出现Table ‘performance_schema.session_variables’ doesn’t exist报错。网上的解决方法是在mysql的bin目录下运行 mysql_upgrade -u root -p --force命令，但是我在输入这个命令之后出现了Error occurred: Cannot select database.报错。

解决方案：

<!--more-->

在mysql文件夹下的my.ini中添加

```ini
[mysqld]
show_compatibility_56 = ON
performance_schema
```

修改之后需要重启数据库。

重启数据库可以按照如下方法：

输出services.msc，点击重启动此服务即可。
![img](https://img2020.cnblogs.com/blog/2015725/202005/2015725-20200526184916096-605326372.png)

然后navicat就可以连接MySQL啦！！

转载：https://www.cnblogs.com/hellowen/p/12967726.html