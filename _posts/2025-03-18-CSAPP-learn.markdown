---
layout:     post
title:      "CSAPP学习记录"
subtitle:   "2025-03-18"
date:       2025-03-18
author:     "Sun"

catalog: true

---
# 主题：CSAPP 学习记录

## 推荐资源

- ⭐⭐康宇PL's Blog——CS基础课不完全自学指南  
  [https://www.cnblogs.com/kangyupl/p/cs-stack-self-study-guide.html](https://www.cnblogs.com/kangyupl/p/cs-stack-self-study-guide.html)  
  - [https://github.com/izackwu/TeachYourselfCS-CN/blob/master/TeachYourselfCS-CN.md](https://github.com/izackwu/TeachYourselfCS-CN/blob/master/TeachYourselfCS-CN.md)  
  - [https://csdiy.wiki/#_6](https://csdiy.wiki/#_6)  
  - [https://github.com/PKUFlyingPig/Self-learning-Computer-Science](https://github.com/PKUFlyingPig/Self-learning-Computer-Science)  

- CSAPP 笔记重点导读  
  [https://fengmuzi2003.gitbook.io/csapp3e](https://fengmuzi2003.gitbook.io/csapp3e)  

- CSAPP 全书笔记  
  [https://www.zhihu.com/tardis/zm/art/455061631?source_id=1005](https://www.zhihu.com/tardis/zm/art/455061631?source_id=1005)  

## 组成原理

**参考耗时**：100h+  
**前置技能**：汇编语言、Linux 常用命令  

我个人认为学习组成原理的主要目标是要搞明白 CPU 内部是怎么工作的，并能够针对现代 CPU 的 TLB、多级缓存、内存屏障等特性写出更优良的代码。

我个人推荐《深入理解计算机系统》（国内俗称 CSAPP）这本书。原教旨派认为学习组成原理应该以实现简单的多级流水线 CPU 为目标，这跟我的着重点不太相同。我更关心程序员可以根据哪些编程原则来更好地利用 CPU 的特性，而 CSAPP 做到了这一点。它真的是在认真教你如何榨取 CPU 性能、如何对自己的程序进行优化，而且还提供了好几个 LAB，专门考察你的理解是否足够深刻。

读完它的前九章就差不多了，其他章节在操作系统课和计算机网络课里会更详细地学习。不过如果想更轻松上手这两门课程，也可以先读一下。学习时也不需要死板地啃一遍，遇到不感兴趣的地方可以跳过。比如我觉得第二章手推浮点数的二进制表达那一堆计算题挺无聊的，所以只是写了一点代码实现了字面上的小数和浮点数间的互转算法就掠过了。

书的作者开过 CMU 15213 这门课，B 站上有人将其全汉化了，有需求可以去看看。

配套 LAB 也是公开在网上的。注意每个实验的源码在压缩包里，参考文档在 writeup 里。

书里面的习题可以不做，但 LAB 是必做的，因为它的设计确实巧妙。比如：  
- **Bomb Lab**：直接扔给你一个可执行文件，让你通过反汇编来 hack 掉它。  
- **Performance Lab**：教你如何运用 CPU 指令并行和 cache，把程序的运行速度提高几十倍，这是别的课程里从未见过的奇妙体验。  

在攻略 CSAPP 的 LAB 的过程中，可以学到的知识包括：  
- gdb 调试  
- 分析程序反汇编码  
- CPU 级的性能优化方法  
- 一点点的 Linux 系统编程  

**来源**：[https://www.cnblogs.com/kangyupl/p/cs-stack-self-study-guide.html](https://www.cnblogs.com/kangyupl/p/cs-stack-self-study-guide.html)
