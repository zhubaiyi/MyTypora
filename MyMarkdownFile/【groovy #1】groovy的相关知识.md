[TOC]



#### 前言

今天看到了许多的groovy语言相关的实用知识，发现这个groovy虽然有自己独立的一套语言体系，但是实际上它跟Java其实相差并不是很大，而且我看跟我同级的大佬也经常在用groovy（2021年大三），因此我认为可以进行相应的知识学习，并且把自己的所获得的知识放到博客里进行分享。（其实我使用csdn发博客只是为了可以巩固我自己的知识，向大家普及知识，如果我够格的话，也只是附带的作用 ）。

在Android学习过程中，Gradle经常被使用。因此，掌握Groovy语言是非常必要的，因为Gradle就是用这种语言编写的，我们需要用这种语言编写任务。以本文为例，开始使用Groovy。本文主要针对有Java基础和一定计算机基础的学生。并且我们这个学期（大三下）也开始学习移动应用开发课程了，因此也更应该多学习一下groovy这个强大的应用工具！

#### 基本概念

Groovy是一种基于JVM（Java虚拟机）的敏捷开发语言，它结合了Python、Ruby和Smalltalk的许多强大的特性，Groovy代码能够与Java代码很好地结合，也能用于扩展现有代码。由于其运行在 JVM 上的特性，Groovy可以使用Java来编写，最终会被编译成xx.class文件在虚拟机中运行。由于它是一种敏捷开发语言，因此很适合用来变现Gradle脚本，因此在Gradle中被广泛运用。（摘自百度百科groovy）

#### 安装教程

##### Windows安装方式：

笔者使用的是Windows操作系统，因此我的使用方法是，直接使用intelliJ IDEA的方式下载就好了。

也可以下载groovy的安装地址，现在完成后在环境变量中进行添加（就跟java JDK的安装方式一样的）。

验证方式是：![image-20210319141450606](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210319141450606.png)

在cmd命令窗口下输入groovy -v，如果出现了版本介绍表明安装成功。



##### MacOS/Linux安装方式：

环境搭建
参考：https://www.bonusbits.com/wiki/HowTo:Install_SDKMan_on_MacOS_or_Linux

```bash
$ curl -s "https://get.sdkman.io" | bash

ps:卸载sdk 
$ rm -rf $sdkHome/.sdkman

```

安装成功后，表示我们可以用sdk 命令来安装groovy了！！！

###### 安装 groovy

```bash
sdk install groovy
```

看到成功后，表示groovy库安装成功。

#### 下载IDEA

https://www.jetbrains.com/idea/download/#section=mac
使用免费版的就可以了！

然而如果你有学生邮箱的话（大学生甚至更好学历就有），可以直接注册使用，然后每年记得再次激活一次就好了。

#### 配置groovy

打开IDEA — 新建Groovy项目 — Groovy library 选择你安装groovy的路径就可以了。
ps:查看groovy路径一般在：`/Users/xxx/.sdkman/candidates/groovy/`

![image-20210319141741937](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210319141741937.png)

进行下一步就可以使用IDEA编辑groovy了！

如果说你问我为什么使用IDEA不适用eclipse，我的想法是eclipse太老了，连安装也不是使用软件的方法，我连JBoss和wildfly也无法使用较高版本，后期也有不少bug，逐渐让我放下了eclipse的使用。







Groovy 语法精讲
groovy 中可以写和java一模一样的代码，同时也可以用groovy的脚本特性，写简单的脚本语言。因为很多特性和java一样，因此这里只挑出和java不一样的地方来讲。

文件结构
在java中，一个class文件的基本结构是：

```java
pacakge xx.xx

import xxxx

class xxx {
    void xxx {
        //do something
    }
}
```

在groovy中，就十分简单了：

```groovy
package xx.xx (这个省了也可以运行，最好是加上，为了规范性)

//do somthing
```

#### 变量类型

groovy既拥有脚本语言的特点，也拥有java的特点，因此它既可以使用弱类型定义变量，也可以使用强类型方式定义变量。示例如下：

```groovy
//弱类型
def x = 10

//强类型
int y = 10
```

groovy中所有的基础类型都会被转换为对应的Class对象，比如：

| 基础类型 | 对象类型  |
| -------- | --------- |
| int      | Integer   |
| char     | Character |
| float    | Float     |
| double   | Double    |
| boolean  | Boolean   |

（表格来自以为段位极高的groovy程序员）

未指定类型的非整数，则会被转换为`BigDecimal`
可用如下式例验证：

```groovy
def a = 0.1
println a.class
```

因此，在groovy中，所有的变量类型都是Object类型！

#### 字符串

groovyz中定义字符串，有三种方式：

##### ‘xx’

这种方式定义的字符串是不可变的，示例：

```groovy
def name ='laosan'
```

##### “xx”

这是可变定义字符串，可以接受变量。示例：

```groovy
def say = "hello, ${name}"
```

##### ’‘xx’’’

这样定义的字符串，允许输入格式。示例：

```groovy
def json = '''\
{
    "name":"winton",
    "age":20
}
'''
```

这样就不用再使用java里的转义字符了.

#### 闭包（我感觉有点像java8中的lambda表达式）

基本结构如下：

```groovy
def name = { params ->
//do something
}
```

示例1：

```groovy
def say = { 
    String word ->
    println word
}
```

示例2:

```groovy
def add = {
    a, b ->
    return a+b
}
```

这个有点类似函数定义。

其他的高级groovy语法或者数据结构我想可以在以后的groovy博客讲解中列出来。



