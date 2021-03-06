# 开题报告展示提纲

## 题目

Linux 内核自动测试与动态差异分析研究

## 研究背景与意义

- Linux Kernel是一个开放自由的操作系统内核，可移植性极强，目前已经成为支持硬件平台最广泛的操作系统。
- Linux Kernel的更新十分频繁，以git repo的形式开源迭代更新，然而各个微小版本之间的差异往往难以明了，特别是一些性能信息往往是难以获取的，所以一些比较分析的工具系统十分有必要。
- Android系统作为当下最流行的移动设备操作系统之一，其内核也是基于Linux Kernel，两者具有相似的一些特点，而如今Android ROM版本众多，性能参差不齐，难以全方位细致地进行比较分析，Linux Kernel的分析系统经改进后可以帮助分析Android ROM镜像的性能指标。

## 研究现状

- Intel公司专注于研究计算机芯片，对于计算机底层有深厚的研究基础。其一个开源项目lkp-tests（Linux Kernel Performance Tests）即旨在能便捷地对Linux Kernel进行一系列典型的性能分析测试。
- kernelci.org是一个开源的针对Linux Kernel的分布式自动测试平台，他们的目标是检测Linux Kernel分支中新的提交代码，在代码并入主分支之前就将可能存在的问题进行报告。
- Instant Bug Testing Service for Linux Kernel(IEEE2013)针对Linux Kernel的Bug存活周期越来越长的问题，提出KIS内核漏洞即时检测系统。
- Testing Linux® with the Linux Test Project(Ottawa Linux Symposium 2002)介绍了LTP这个组织作为平台贡献的大量测试Linux内核的自动化脚本，包括但不限于C、Perl、Shell语言，促进了其他开源社区及企业对Linux Kernel测试的关注与贡献

## 研究内容方案

- 首先经过老师接洽，我会向Intel的工程师详细学习相关的技术细节，包括如何利用测试工具提供的不可读的数据结果，如何搭建整个分发编译系统等，然后把整个系统进行复现。
- 其次在熟练掌握并理解原分析系统并且了解Android ROM特征特性的基础上，根据需要修改代码使之能适配对Android ROM的分析。
- 在其他工作完成得较为充分的情况下，可以针对系统测试的庞杂信息进行数据挖掘，发现潜藏的有意义的内容，比如：分析内核工程师的工作重心，提前预测接下来的重大特性。

## 工作基础

### 目前已经完成的工作：

- 基本跑通lkp-test项目的大部分测试模块
- 阅读分析了一部分项目源码
- 大致了解了测试结果数据的形式与特点

### 学习的相关知识

- Linux Kernel目录结构与大致作用
- Linux下系统工具Perf、Sar等
- 系统测试常用的一些脚本工具，比如Shell、Perl等

## 预期成果与进度安排

期望最终能在复现Intel整套系统的基础上，完成针对Android ROM的新系统，并能顺利进行测试、比较、分析。

- 2016.1 - 开题后，尝试搭建kernelci，并继续阅读分析lkp-test源码
- 2016.1 - 2016.2 前往上海Intel公司学习相关技术细节，写出详细的kernelci.org和lkp-test技术分析报告和测试运行报告，并对二者进行分析比较
- 2016.3 - 2016.4 尝试复现原系统，并进行针对Android ROM的修改
- 2016.5 - 2016.6 完善系统，尝试进行数据挖掘，撰写毕业论文
