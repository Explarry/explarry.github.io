---
layout: post
title:  operation system
categories: operation_system
---
# 1 操作系统的历史

* 多任务处理是操作系统诞生的驱动因素，或者说操作系统解决的问题是如何高效地进行多任务处理

  如果单任务独占，那么不需要操作系统

  发展的进程：

  单任务独占 --> 批处理 --> 多任务处理

* 硬件上

  * 处理器的进步使得计算效率大大提升
  * 内存的增大使得计算机同时装载多个程序成为可能

* 对 cpu 进行分时复用的关键技术是中断

* 虚拟化的目的是提供优秀的 api，让程序的功能得以实现，并且在使用时好像是在独占设备资源

* three easy pieces

  * 虚拟化

    进程，虚拟内存，设备抽象

  * 并发

    cpu 的分时复用，进程/线程间的通信

  * 持久化

    文件系统



# 2 应用眼中的操作系统

* coreutils

  体积更小的替代品，busybox

* ubuntu packages 支持文件名检索

  当系统缺少某些东西时，这是一个非常好的检索入口

* elf

  executable linkable format，可执行的可链接的格式

  * xxd，反汇编命令，可以用来分析 elf 格式的文件
  * readelf，可以用来查看 elf 格式的文件的信息