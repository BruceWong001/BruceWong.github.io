---
layout:     post
title:      Scrum模式之估算点模式读后感 
subtitle:   
date:       2021-11-14
author:     Bruce Wong
header-img: img/pexels-jonathan-petersson-965879.jpg
catalog: true
tags:
    - 敏捷
    - Agile
    - Scrum Patterns
    - 随笔
    - ProductOwner
    - User Story
---

估算一直都是软件开发中一个无法绕过的难点之一。项目预算和风险把控需要有一个估算，产品发布时间预测需要估算作为参考。而人类最不擅长的就是估算，毕竟这个是还没有发生的事。我在平时工作中也经常面临要对产品Release或者投标的标书进行估算的场景。最近看了Scrum Pattern中关于估算模式的文章，这篇文章主要说明的是使用估算点数(Estimation Point)的方法，虽然最近几年已经证实这种方式很难落地，但是它可以作为我们认识传统人天这种绝对估算弊端的入口，以及相对估算的优势。所以从中我们可以发现平时估算不准确的一个原因。这里主要总结的是我的读后感，希望分享给小伙伴们一起学习。文末有原文链接，感兴趣的小伙伴可以精读一下，欢迎大家一起交流。  
### 认识到估算无法准确  
很多时候客户都希望看到符合或超过他们预期的评估；干系人期望的评估总是会让团队感到痛苦。如何让团队可以有节奏地保持一定的产出速率是估算的一个结果，也是估算可以影响到的一个因素。当然估算就是一种假设，无法达到精确预测的作用。评估本身就是基于以往的经验做出的一个合理但不确定的假设。但是如果花费太多时间来做估算，往往是得不偿失的，同时也会让团队在反复的评估中变得麻木。  
### 我们无法做到有效工作40小时  
产品负责人或者项目经理一般都希望能够团队提供对于一组功能的评估，通常是可能的交付日期。例如比较自然的方式是对每一个功能做评估，最后将这些相加得到一个交付的最终日期。很多时候会通过评估功能的工作总数除以每周工作40小时来得到潜在的交付日期。不过这块会有一个小问题，其实并不是每个人的每周工作都是40小时。例如有开会的时间，处理邮件的时间，管理的时间，切换工作上下文的时间，甚至评估本身也是时间。而这些综合到一起每个人几乎最多只能有一半的时间在实际工作中。但是我们很多人可能根本没有意识到这个认知差距。这也是很多时候估算不准确的一个原因。  

我们要认识到估算并不是承诺，如果我们给出了人天等具体时间，接收信息的人会不自觉地认为这就是一个承诺。团队要不顾一切的兑现承诺。很多时候大家会在绝对评估的数字上忽略了理想和现实的差距。当然你会说我们会打上一些buffer time。例如加20%的作为无法40小时工作的额外补充时间。很多时候你会发现这个buffer time还是不够，或者过多，最终还是会导致干系人对团队评估的的不信任。  

那就是说我们不要估算了吗？当然也不是，彼得德鲁克说过：你想要个改进一个东西，就需要先能度量他。所以估算的目的是为了通过度量找到改进的空间，持续提高团队能力。当然这一度量可以伴随一些副产品，其中之一就是我们团队产能的评估。  

### 为什么相对估算优于绝对估算  
了解敏捷的人应该都知道绝对估算和相对估算的区别。当使用绝对估计时，我们用于估计的单位意味着相应的持续时间。例如人们可以对100米跑道的长短达成一致，但他们很难对跑完100米跑的时间达成一致。毕竟每个人能力不同，我们不能都是苏炳添，哈哈。不过你会惊奇的发现大家都同意跑200米可能要比跑100米花两倍多的时间，这就是相对评估可以快速达成一致的一个例子。找到一个大家都能理解的简单的事情作为基线，之后基于基线做相对估算。  

### 相对估算的一个使用场景  
基于上面的这个例子，想想我们平时的工作，团队需要找到一个基线任务作为100米跑的持续时间。不需要具体时间，只是做这件事，当然前提是这个工作最后达到完成标准(DoD)。因为每个人实际完成这件事的时间都会不一样。例如最简单的一种方式，一个Team曾经在之前某次Sprint中做过的功能，作为一个大家公认的基线任务。那么使用相对评估，任何待评估的工作大家先认可这个基线任务的体量、技术复杂度、业务复杂度等因素。然后让团队基于这三个因素相对于基线对新的任务进行评估。新任务是基线任务的几倍，如果把基线任务设定为1 Point，那么新的任务如果是3倍的话就是3 Point。要得到大家对这个评估一致认可，我们引入了著名的德尔菲法。每个团队成员自己思考给出答案，如果出现差异，在成员之间讨论差异。而德尔菲法的最简单用法就是使用敏捷估算扑克。就像在打德州扑克一样大家在同一时间揭开自己的底牌。同时为了体现估算并不是线性增长的，随着技术或者业务复杂度的提升整体估算的不准确性会呈指数级增加，敏捷估算扑克又加入了斐波拉契数列来体现这种非线性增加。  
### 相对估算的一个特殊场景  
在这个Scrum Pattern中给出了一个想法，我认为属于相对估算的一个特殊场景。如果我们应用好分拆故事的技术，将每个Story都拆分成接近于基线任务，那么这会让评估更高效和相对准确，因为每个故事都是Team熟悉的体量、技术和业务复杂度。Team从经验和自信程度来说都是更有把握的。那么这种场景的估算就只是数任务个数就可以得到一个你想要的估算了。  

### 估算区间的作用  
另一个在该模式中提出的一个是乐观和悲观估算。也就是每一个估算鼓励Team给出两个值，一个是乐观的一个是悲观的，而这两个值可以让最终的整体估算得到一个区间。这个区间就是潜在的可能交付区间。拿上面的例子来说明，如果一个Team在一个Sprint中乐观估算能够完成10 Point的任务，悲观估算进能够完成4 Point的任务，那么最终我们可以推算出总数是20 Point的任务需要2~5次Sprint来完成的区间。通过区间来给干系人表明：这是一个估算而不是承诺；另外团队会尽量去实现乐观的评估的交付时间，但是仍然存在悲观评估的可能，我们需要一起来承担风险。  

## Bruce有话说  
文中一样提到了估算点模式只是一种方式，最近几年也兴起了“无估算”方式来代替，不过无估算并不是真的不需要估算，而是不需要复杂的估算方法(上面提到的数用户故事个数的方式就是一种"无估算"方式)。如果使用估算扑克的估算方式需要花费很长时间来操作，那么该方法显然也不适合你的团队。Team需要找到适合自己的方式。估算的结果是我们想要一个可以用来度量的数字——度量团队的产能，度量可以交付的时间等。不过估算的过程其实更为重要，一个高效的过程，其中不只是开发人员，而是几乎所有相关的人员会进行头脑风暴，尝试达成一致，发现潜在的风险，提出可行的方案。最终团队在这个过程中磨合并成长。这才是这个估算点模式的价值所在。  

我也总结过如何进行有效的落地估算方式，大家可以参考阅读《[如何进行用户故事估算](https://brucetalk.com/2021/10/10/storypoint_estimation/)》这一篇文章。  

## 参考引用  
- [Estimation Points](http://scrumbook.org.datasenter.no/value-stream/estimation-points.html)
