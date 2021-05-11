---
title: Node重装系统后的配置环境变量
categories: node
tags: 
  - git
  - hexo
  - node
---

**[Node重装系统后的配置环境变量]**
<!--more-->

1 将node加入到环境变量的path中  D:\IDE\nodejs;
D:\IDE\nodejs\node_global

2设置npm的全局模块的存放路径以及cache的路径 !

![image-20200929220126037](C:\Users\yan13\AppData\Roaming\Typora\typora-user-images\image-20200929220126037.png)

npm config set prefix "D:\IDE\nodejs\node_global"

npm config set cache "D:\IDE\nodejs\node_cache"

检验是否成功

![image-20200929220345751](C:\Users\yan13\AppData\Roaming\Typora\typora-user-images\image-20200929220345751.png)