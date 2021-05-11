---
title: 手动添加右键菜单没有Git Bash Here
categories: git
tags: 
  - git
  - hexo
---

# [手动添加右键菜单没有Git Bash Here](https://www.cnblogs.com/ql123456/p/12119135.html)

 小编电脑出了问题，于是重新安装的系统，装好之后发现右键的git bash here 命令没有，于是手动实现添加命令行

## 第一步 WIN + R 打开cmd命令行，输入‘regedit’，打开注册表

## 第二步 进入[HKEY_CLASSES_ROOT\Directory\Background]

<!--more-->

![img](https://img2018.cnblogs.com/i-beta/1487613/201912/1487613-20191230122613078-1647391975.png)

 

## 第三步 在[shell]下右键-新建项[open in git ](名字任意，但最好是git bash here)

## 　设置其值为“Git Bash Here",此为右键菜单显示名称。

   此时鼠标右击就能看到Git Bash Here,但是没有关联程序 即现无实际作用

## 第四步 在[open in git]下右键-新建-项[command],其值为 "git安装根目录\bin\bash.exe" --login -i

![img](https://img2018.cnblogs.com/i-beta/1487613/201912/1487613-20191230123454429-324828237.png)

## 第五步 为了能和第一次安装一样，右键能看到Git的小图标。

在open in git中右击-新建-字符串值，名称为Icon,右键编辑 其值为“git安装根目录\mingw64\share\git\git-for-windows.ico”。

最后的目录结构为：

![img](https://img2018.cnblogs.com/i-beta/1487613/201912/1487613-20191230123441126-834381785.png)

 

 好了，按照以上操作大功告成！

转载：https://www.cnblogs.com/ql123456/p/12119135.html