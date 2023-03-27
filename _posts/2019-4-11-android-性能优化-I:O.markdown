---

layout: post
read_time: true
show_date: true
title: "android-性能优化-I/O存储优化"
date:  2019-4-11 22:31:49 +0800
img: posts/20210402/post7-header.webp
tags: [Android,Performance Improving]
category: Android
author: cs
description: "android-性能优化-I/O存储优化"

typora-root-url: ../../flywithwater.github.io
---

因为磁盘I/O很耗时，所以，I/O部分的总体优化原则是：

​	 能不磁盘I/O就不磁盘I/O，必须磁盘I/O就尽量顺序读取，且视情况实现并行I/O和异步I/O；

具体见下图：

![Android-IO](/assets/img/posts/Android/Android-IO.png)

