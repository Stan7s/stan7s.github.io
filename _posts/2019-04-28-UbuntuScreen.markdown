---
layout: post
title:  "Ubuntu Screen命令"
date:   2019-04-28 16:10:00 +0530
categories: ["research"]
---

在Linux中，我们可以使用screen来使用多个屏幕，这样使用起来会非常的方便。

[http://www.ibm.com/developerworks/cn/linux/l-cn-screen/](http://www.ibm.com/developerworks/cn/linux/l-cn-screen/)
这个是一个screen的文档。


这里介绍一些自己使用的best practice.

1. screen -S name 启动一个名字为name的screen
2. screen -ls 是列出所有的screen
3. screen -r name或者id，就可以回到某个screen了
4. ctrl + a + d 可以回到前一个screen，当时在当前screen运行的程序不会停止

引用自：[https://blog.csdn.net/luoyouren/article/details/51382710](http://www.ibm.com/developerworks/cn/linux/l-cn-screen/)