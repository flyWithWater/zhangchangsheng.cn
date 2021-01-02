---
layout: post
title:  "android-性能优化-I/O存储优化"
date:   2019-4-11 22:31:49 +0800
categories: Android

typora-root-url: ../../flywithwater.github.io
---

因为磁盘I/O很耗时，所以，I/O部分的总体原则是：

​	 能不磁盘I/O就不磁盘I/O，必须磁盘I/O就尽量顺序读取，且视情况实现并行I/O和异步I/O；

具体见下图：

![Android-IO](/assets/Android/Android-IO.png)

