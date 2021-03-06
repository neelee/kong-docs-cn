# 欢迎使用kong

> 本文原文链接：https://docs.konghq.com/1.1.x/getting-started/introduction/

> 开始之前，确保已经安装好Kong —— 只需要花一分钟的时间。

在你深入学习Kong之前，确保你已经知晓它的目标和设计理念。一旦您熟悉Api网关的概念，本指南将为您介绍如何使用Kong，以及一些基本操作，比如:

- 运行Kong实例
- 添加和消费Services
- 在Kong上安装插件

## 从技术角度来看，什么是Kong？
您可能已经听说过Kong基于Nginx，利用了其稳定性和高效率。但这究竟是怎么实现的呢？

更确切地说，Kong是一个在Nginx中运行的Lua应用程序，并且可以通过lua-nginx模块实现。Kong不是用这个模块编译Nginx，而是与OpenResty一起分发，OpenResty已经包含了lua-nginx-module。OpenResty不是Nginx的分支，而是一组扩展其功能的模块。

这为可插拔架构奠定了基础，可以在运行时启用和执行Lua脚本（称为“插件”）。
因此，我们认为Kong是**微服务架构的典范**：它的核心是实现数据库抽象，路由和插件管理。
插件可以存在于单独的代码库中，并且可以在几行代码中注入到请求生命周期的任何位置。

## 下一步

现在，让我们熟悉学习如何“开始”和“停止”Kong。
点击进入[5分钟快速开始Kong](quickstart.md)
