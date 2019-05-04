---
layout: post
title:  "引用Google Font"
date:   2019-05-04 21:39:00 +0530
categories: ["work"]
---

觉得博客标题有点过于正常，于是入坑了Google Fonts。

首先在[https://fonts.google.com](https://fonts.google.com)挑选字体。

以 Gloria Hallelujah 这款字体为例：
![GoogleFont-1]({{site.url}}/pic/GoogleFont-1.png)

在html上引用：
'''
<link rel='stylesheet' type='text/css' href='https://fonts.googleapis.com/css?family=Gloria Hallelujah'>
'''
注意是 https 不是 http。

修改css文件：
'''
font-family: 'Gloria Hallelujah','PT Sans';
'''
在后面保留了原先的字体，这样就算前面的挂掉也不至于回到Times New Romen（不

刷新，成功~
![GoogleFont-2]({{site.url}}/pic/GoogleFont-2.png)