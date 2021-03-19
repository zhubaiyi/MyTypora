#### 前言

在groovy第一解决的讲解中已经讲到，使用idea可以进行groovy的程序运行。以下是创建一个groovy工程的方式：

![image-20210319143335579](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210319143335579.png)

点击确定后可以产生新的窗口：

![image-20210319143359583](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210319143359583.png)

注意这里完成了一半，在新的窗口中点击文件——>file structure->module在src文件夹里新建两个文件夹groovy和java，用于区别两个语言的不同，将两个文件夹都设置为源。

![image-20210319143923469](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210319143923469.png)

创建一个groovy文件

写如下内容：

```groovy
package learn

/**
 * Created by zby on 2021/may/19
 */
class LearnGroovy {
    static void main(args){

        println "Hello World!";
    }

}
```

点击编译就可以成功编译出groovy编写的代码了。