---
layout: post
title:  "Cminus词法扫描实验"
date:   2019-05-03 23:54:00 +0530
categories: ["work"]
---

画了一个贼好看的DFA。

![Cminus-DFA]({{site.url}}/pic/Cminus-DFA.png)

如上图所示，此DFA共包含11个状态，其中除START（初态）和DONE（终态）外，可分为以下三类：

1. 注释相关的状态：DORC（Divide OR Comment，可能是除号，也可能是注释的开始），INCOMMENT1（进入注释），INCOMMENT（可能结束注释）。由于C-的注释较TINY而言略为复杂，因此需要设计多个中间状态以确保能够正确识别；
2. 变量或整数相关的状态：INID（变量名），INNUM（无符号整数）；
3. 运算符相关的状态：INMORE（大于或大于等于），INLESS（小于或小于等于），INNEQ（不等于），INEQ（等于或赋值）。

除此之外，单字符运算符（包括加减乘除、分号、逗号、括号等）可以直接由初态转移到终态；空格、制表符、换行则可直接忽略。
