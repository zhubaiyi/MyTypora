最近在用Typora写笔记，想要像新建一个Excel或者tex文件一样直接鼠标右击新建一个md文件。Typora是一款非常好用的MarkDown操作软件。
网上方法很多，这是最简单的一个。

```

Windows Registry Editor Version 5.00
[HKEY_CLASSES_ROOT\.md]
@="Typora.exe"
[HKEY_CLASSES_ROOT\.md\ShellNew]
"NullFile"=""
[HKEY_CLASSES_ROOT\Typora.exe]
@="Markdown"
```

第二步 将这个txt文件另存为reg格式

第二步 将这个txt文件另存为reg格式，就怕有人不会另存为，还是贴个图片吧

第一步：新建一个txt文档，将下面的内容复制进来。



第三步 将生成的reg文件双击运行一下，全部点击确定就可以了
说明一下 这里的Markdown可以自定义，在上面的复制内容中@=“Markdown”，这里的@=“这里可以自定义”，Ok了