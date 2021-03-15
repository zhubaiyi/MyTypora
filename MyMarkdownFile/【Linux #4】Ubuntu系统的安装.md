# 【Linux #4】Ubuntu系统的安装

[^2020/may/15]: 第一次编辑

​		自从学习了Linux系统之后我的生活变法上了重大的变化（指需要花费大量的时间用于学习自己从来没接触到的东西），不过老师也是比较不错，课上使用的是Ubuntu系统，相比于CentOS是比较不错的。以下是2种常用的方式。



## （1）使用虚拟机进行安装

### 使用工具：

强烈建议使用Vmware，不花钱，去官网https://www.vmware.com/即可下载。不建议使用VirtualBox。VMware工具更加强大，最简单的来说，可以使用Windows跟虚拟机之间的复制粘贴，virtualbox就不行。

### 安装方法：

首先下载ubuntu的镜像文件。

这个直接去官网http://www.ubuntu.com/download/desktop/zh-CN进行下载，有不同版本的，建议下载版本号为18开头的iso镜像文件，版本为20的太新，很多资源使用不了，而16的则太旧，镜像文件在新建虚拟机的时候是需要的，后期就不需要了。

如果发现下载的很慢，可以找到国内的镜像源进行下载。

去官网https://www.vmware.com/即可下载VMware，使用虚拟机VMware即可安装虚拟机。

![image-20210315174157396](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174157396.png)

下载速度很快，中规中矩的安装完成。界面如图：

![image-20210315174326972](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174326972.png)

完成之后，点击右侧部分的新建虚拟机。点击自定义。

![image-20210315174400797](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174400797.png)

下一步。

![image-20210315174435855](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174435855.png)

点击安装程序映像文件，找到自己下载到的iso镜像文件。点击下一步。

![image-20210315174450009](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174450009.png)

下一步，为自己的虚拟机起名字，对自己的用户起名字，并设置密码以后登陆虚拟机会用到，如果嫌麻烦，可以在登陆后点击设置进行免密码登录。

![image-20210315174657524](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174657524.png)

点击下一步，选择位置。建议安装在其他盘，毕竟C盘的资源很珍贵

![image-20210315174815591](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174815591.png)

这里如果嫌慢，可以增加处理器数量。

![image-20210315174840182](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174840182.png)

选择内存大小阶段，可以随意设置，建议使用建议大小。

![image-20210315174919830](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174919830.png)

使用nat方式进行网络交换。

![image-20210315174936427](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174936427.png)

点击推荐的，直接下一步。

![image-20210315174949797](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315174949797.png)

这个无所谓，选择推荐的。

![image-20210315175022693](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175022693.png)

使用推荐的。

![image-20210315175036901](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175036901.png)

这里不变

![image-20210315175050087](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175050087.png)

![image-20210315175101204](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175101204.png)

![image-20210315175109920](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175109920.png)

之后就会安装成功。

![image-20210315175209691](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175209691.png)

之后就静静等待安装完毕吧。这个过程需要花很长时间。

![image-20210315175250155](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175250155.png)

后期就直接可以安装了，由于笔者C盘内存不够，就不截图了。

接着就会到达图形界面的窗口，稍等一段时间后，会让你注册，只要好好注册就行。

这样就可以了。

如果发现有黑屏现象，详情解决方法请参见文章<https://blog.csdn.net/edc370/article/details/81913420>可以进行解决。

最后界面是这样。

![image-20210315175711700](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315175711700.png)

上来之后第一件事就行把源换成国内的。

本版本是20的请参见文章https://blog.csdn.net/wangyijieonline/article/details/105360138的解决方法

本版本是18的请参见文章https://blog.csdn.net/qq_43619461/article/details/109078324的解决方法

本版本是16的请参见文章https://blog.csdn.net/wzyaiwl/article/details/88571414的解决方法

（2）直接在Windows中安装双系统

打开你的Windows商店，搜索Ubuntu即可下载

![image-20210315180040141](https://raw.githubusercontent.com/zhubaiyi/MyTypora/main/img/image-20210315180040141.png)

这种方法的好处就是比虚拟机加载更快，可以直接在自己的电脑上进行文件编辑，在使用Ubuntu进行运行。

因为笔者使用的是虚拟机的方式，因此详情请参见B站的三个视频，有具体的讲解：

https://www.bilibili.com/video/BV1kz4y167G6

https://www.bilibili.com/video/BV11T4y1T75K

https://www.bilibili.com/video/BV19U4y1x7gF

以上就是安装Ubuntu的具体方式了，希望你可以变得更强，顺便请积极讨论反馈，你的加入就是对我最大的支持。