#! https://zhuanlan.zhihu.com/p/682212426
# 容错量子计算学习导论-Overview
- We have learned that it is possible to fight entanglement with entanglement. - John Preskill
- To be an Error and to be Cast out is part of God's Design. - William Blake

## 前言
在这一章节，我主要学习一些关于量子纠错的基础知识。书本中主要围绕 quantum error-correcting codes, fault-tolerant quantum computation, and the treshold theorem 展开。Quantum error-correcting codes能够通过encoding，使得量子态编码为具备抗噪能力，同时通过decoding，使得量子态复原。前几节将介绍一些quantum error-correction的基本定理以及常见示例。由于encoding和decoding通过量子门操作实现，但有时无法保证操作的完美，因此fault-tolerant quantum computation 中移除了encoding和decoding操作完美的假设。同时threshold theorem 指出当量子门的噪声小于某个阈值，则存在方法有效实现任意规模的量子计算。

注意，阅读笔记，仅仅用于快速了解这本书中的量子纠错知识，不等同于了解量子纠错，还有更多资料值得学习。

——2024年9月20日更新：

在之前计划将QCQI这本书里面的QEC内容进行学习，但是这里面的内容实在过于经典和老套，像是写在教材书上的知识。目前大多量子纠错的内容从论文中看的更多，后续考虑更新一些note或者整理的基础知识。QCQI后续有时间可以继续更新。

——2024年11月9日更新：

这个内容我非常想做，但是最终还是拖沓了很久，但我基本上这一年都在这个容错量子计算这个领域学习。

我尝试寻找这个原因可能是：
1. 懒+其他事情太多，这件事件的优先级不高。还有更多事情需要做，在读的研究生和博士生应该都能理解吧[哭]。优先级不高，体现在本身做成这件事情，对于我目前来说，帮助其实不是很大。因为，我很明确自己的最重要的事情是需要尽可能花时间在做科研，写成论文的形式发表，让小领域的人能够认可。

2. 质量和精力难以权衡：我不希望我只做简单“copy”和“注释”，但也很难做到像论文一样，完全的自己思考和撰写，太耗精力并且收获甚微。我更希望撰写一个通俗易懂的导论，能够让人快速阅读的。对于我的时间和精力的要求还是蛮高的，需要我将QCQI那本书的相关内容阅读清楚，同时还可能需要阅读一下其他的资料内容。

3. 不太符合目前的学习状态。我本人现在的学习风格，偏向于做科研的风格，基本上是阅读大量的论文，寻找问题，把必须学习的知识学习到，接着就是寻找方法和策略（在自己熟悉的领域）。（这种风格很像打竞赛的感觉，快速且准确的学习，然后完成一个任务）难以沉下心，去阅读一些短期、论文内可能用不到的知识，导致我其实不太注重于太基础的阅读，认为是耗费时间的。

当然，原因始终是借口，最终的结果还是没有更新。我希望把这个内容给捡起来，但是更新的速度可能相对来说，每周我只能抽出周六、周末的一个或者两个下午的时间。

量子计算或者容错量子计算领域中的小方向纵多，知识浩瀚，并且还在不断的更新和迭代中。

关于后续的想法，我想先调研一下：
1. 容错量子计算方面的教程，大概选择几个，整合一个叙述逻辑，通过根据该知乎文章+github示例代码开源的形式，撰写一个类似容错量子计算领域的导论形式，帮忙快速入门容错领域。
2. 自己的能力是有限的，更多可能做一个整合现有的优秀自学资料的身份。打算仿造https://csdiy.wiki/ ，构建一个qsdiy.wiki，https://github.com/kechen666/qc-self-learning 。（想法萌发，正在构建中）

我希望尽量在我研究生毕业，读博之前撰写完成。

## 目录
- [Basic idea of Quantum Error Correction](https://zhuanlan.zhihu.com/p/682212302) (持续更新中。。。)
<!-- - [Theory of Quantum Error Correction] (准备中。。。) 


## 其他学习资料

### Video: 
1. Quantum error correction (QEC) Tutorial -1| Kishor Bharti, Youtobe: https://www.youtube.com/watch?v=yEVJcEC34rw&list=PLD9iE8dbH_2VT2mgoeEXfswH52QN3Y2cf -->
