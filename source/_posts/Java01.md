---
title: Java01
categories: Java
tags: 
  - java
  - 语言
  - 面向对象
---

### 软件开发介绍

**软件开发**
软件，即一系列按照特定顺序组织的计算机数据和指令的集合，有**系统软件**和**应用软件**之分。
<!--more-->

**人机交互方式**

- **图形化界面**(**Graphical User Interface GUI**)这种方式简单直观，使用者易于接受 ，容易上手操作。
- **命令行方式**(**Command Line Interface GUI**)：需要有一个控制台，输入特定的指令，让计算机完成一些操作，较为玛法，需要记录住一些命令。

`Pascal之父Nickiaus With:"Algorithms+Data Structures=Programs"`
`施乐-苹果-微软`

**常用的DOS命令**
dir：列出当前目录下的文件以及文件夹
md：创建目录
rd：删除目录
cd：进入指定目录
cd..：退回到上级目录
cd\：退回到根目录
del：删除文件
exit：退出 **dos** 命令行
*echo   javase>1.doc：将“javase”写入到1.doc文件里面
**常用快捷键**
左、右：移动光标
上、下：阅览历史操作命令
Delete和Backspace：删除字符

### 计算机编程语言介绍

**什么是计算机语言**
计算机语言：人与计算机交流的方式
如：**C、C++、Java、PHP、Kotlin、Python、Scala等**
第一代语言
机器语言：指令以二进制代码形式存在。
第二代语言
汇编语言：使用助记符表示一条机器指令。
第三代语言：高级语言
C、Pascal、Fortran面向过程的语言
C++面向过程/面向对象
Java跨平台的纯面向对象的语言
.NET跨语言的平台
Python、Scala...

### Java语言概述

是**sun (Stanford University Network，斯坦福大学网络公司)** **1995**年推出的一门高级编程语言。
是一种简单易用、完全面向对象、与平台无关、安全可靠、主要面向Internet的 开发工具。
已经成为Web应用程序的首选开发语言。
`后台开发：Java、PHP、Python、Go、Node.js`
**Java技术体系平台**
Java SE
`支持面向桌面级应用`
Java EE
`是为开发企业环境下的应用程序提供的一套解决方案，主要针对Web应用程序开发`
Java ME
`支持Java程序运行在移动终端上的平台`
Java Card
`支持一些Java小程序运行在小内存设备上的平台`

**Java 应用领域来分：**
企业级应用
Android平台应用
大数据平台应用
移动领域应用

**Java语言的诞生**
java之父：James  Gosling
java十余个纯粹的面向对象的程序设计语言，舍弃了C语言中容易引起错误的指针，增加了垃圾回收器功能

**Java的主要特征**
易学的；
强制面向对象的；
分布式的；
健壮的；
安全的
体系结构中立的
解释型的
性能略高的
原生支持多线程的

### Java程序运行机制及运行过程

**Java语言的特点**
面向对象
`两个基本概念：类、对象`
`三大特性：封装、继承、多态`
健壮性
`吸收了C/C++语言的优点，但去掉了其影响程序健壮性的部分，提供了一个相对安全的内存管理和访问机制`
跨平台的
`跨平台性：通过Java语言编写的应用程序在不同的系统平台上都运行：“Write once，Run Anywhere”`
`原理：只要需要运行Java应用程序的操作系统上，先安装一个Java虚拟机（JVM Java Virtual Machine即可。有JVM来负责Java程序在该系统中的运行。`

**Java两种核心机制**
Java虚拟机（Java Virtual Machine）
垃圾收集机制（Garbage Collection）

**核心机制----Java虚拟机**
JVM是一个虚拟的计算机，具有指令集并使用不同的存储区域。负责执行指令，管理数据、内存、寄存器。

**核心机制----垃圾回收**
不再使用的内存空间赢回收----垃圾回收
垃圾回收在Java程序运行过程中自动进行，程序员无法精准控制和干预。

### Java语言的环境搭建

**JDK、JRE**
JDK（Java Development Kit		Java开发工具包）
`JDk包含了java的开发工具，也包括了JRE`
JRE（Java Runtime Environment		Java运行环境）
`包括Java虚拟机和Java程序所需的核心类库等`
JDk = JRE + 开发工具集
JRE = JVM + Java SE 标准类库

**下载并安装JDK**
网址：www.oracle.com、www.java.sun.com
安装：下一步即可
			安装路径不要有中文或者空格等特殊字符
环境配置：略

### 注释（Comment）

单行注释
多行注释
文档注释（java特有）

### Java API文档

API（Application Programming Interface，应用程序编程接口）是Java提供的基本编程接口
http://www.oracle.com/technetwork/java/javase/downloads/index.html
Additional Resources-Java SE 8 Documentation下载

`观看尚硅谷的视频写得笔记`