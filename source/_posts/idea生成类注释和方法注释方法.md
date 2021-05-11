---
title: idea生成注释的方法
categories: 软件的使用
tags: 
  - idea
  - 软件使用
---

> 最近从eclipse转idea了，第一步当然是配置快捷键，模板等。但是！发生了一件贼蛋疼的事情，竟然一直找不到正确添加方法注释的方法！ 最后自己摸索到了，在此详细记录，供大家参考。

```
测试版本为idea for mac，可能快捷键不同，但是设置等肯定是相同的
1
```

------

<!--more-->

## 生成类注释

1. 打开Preferences
2. Editor -> File and Code Templates -> Files -> Class 
    ![这里写图片描述](https://img-blog.csdn.net/20171101005538072?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
3. 效果图 
    ![这里写图片描述](https://img-blog.csdn.net/20171101010225755?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
    网上很多都是在Includes的File Header里面添加，在这里面添加还需要自己去移动下鼠标，然后再去操作键盘，再去写description，，直接在创建类的时候就添加好description不更快吗？
    - **在此添加的话你每次创建类的时候会弹两次框，第二次是让你输入description的内容了**，so, 这就是最优的方法
4. 同理，也可以在这儿为你的Interface，Enum添加上注释

### 生成类注解模板

```
/**
* @program: ${PROJECT_NAME}
*
* @description: ${description}
*
* @author: Mr.Wang
*
* @create: ${YEAR}-${MONTH}-${DAY} ${HOUR}:${MINUTE}
**/123456789
```

> 这里的代码区显示有问题，csdn有bug ，去掉里面的中文就行了。

------

## 生成方法注释

1. 打开Preferences
2. Editor -> Live Templates -> 点击右边加号为自己添加一个Templates Group -> 然后选中自己的Group再次点击加号添加Live Templates 
    ![这里写图片描述](https://img-blog.csdn.net/20171101011618802?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
    ![这里写图片描述](https://img-blog.csdn.net/20171101011634942?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
3. 然后设置自己喜欢的快捷键 在Abbreviation里面 记得在Applicable in 里面勾选,起码也要勾选class 
    ![这里写图片描述](https://img-blog.csdn.net/20171101011646159?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
4. 然后在Edit variables里面添加参数和返回值的自动取值 
    ![这里写图片描述](https://img-blog.csdn.net/20171101012257865?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
    Expression里面选择就是了 
    ![这里写图片描述](https://img-blog.csdn.net/20171101012441585?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
5. 然后再你的方法上面直接输入/ + 你设置的Abbreviation快捷键 + tab键就直接生成了 （我设置的是/+ a + tab） 
    效果图： 
    ![这里写图片描述](https://img-blog.csdn.net/20171101012859816?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzQ1ODExMTg=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
    里面的参数和返回值都是根据你在Edit variables里面添加的自动生成的，

### 生成方法注解模板

```
** * @Description: $description$ * @Param: $params$ * @return: $returns$ * @Author: Mr.Wang * @Date: $date$ */ 
```

> 注意，这个和类注解模板有点不一样，这个是用两个$$ ，这个的作用就是生成后光标直接跳到当前位置，这样也可以直接去输入description的内容了
>
> 对于 Live Templates只能说真的很强大，你平常用的sout ,psvm什么都是里面的，大家可以自行百度一下学习一下。

版权声明：本文为博主原创文章，遵循[ CC 4.0 BY-SA ](http://creativecommons.org/licenses/by-sa/4.0/)版权协议，转载请附上原文出处链接和本声明。

本文链接：https://blog.csdn.net/qq_34581118/article/details/78409782

