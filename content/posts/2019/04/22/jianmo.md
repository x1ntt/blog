---
title: "关于一次数学建模"
date: 2019-04-22T16:11:36+08:00
tags: ["生活","比赛"]
categories: ["生活"]
---

　　这两天在参加一个`数学建模`的比赛，我觉得也许应该把这样的经历写下来，也许可以引发思考。

　　数学建模其实并不是计算机类的比赛，但是我觉得这个比赛还不错，让我觉得不错的地方就是它的规则：

+ 并不会限制你用什么方法完成题目（没有百度的我是一个不完整的我）

+ 限制时间（真的能够激发我的速度）在比赛的时候真的能感觉大脑在发热 那就是思考的感觉（坚信）

　　我去看过其他博主的参加建模的经历，他们那样的比赛是很认真的那种 会很投入 但是我们学校的建模比赛给我的感觉就是，一个人的比赛（大概是因为学校弱吧，但是我真得想想为什么只能在这里上学）。因为每次都找不到好的队友，或者说不会搭配队友

　　比如说今年的省赛我就是随便找的队友，倒不是说我不认真，主要是真的找不到合适的队友，我本身就只会写代码，我的数学能力很差，所以基本上我都只能做那个计算机类的题目，但是这样的话，就没人能够和我讨论了。

　　所以基本上建模和编程都是我一个人，不过好在今年论文我倒是没有太参与论文的写作，仅仅是写了思路以及解题步骤（去年基本上就是我一个人把三个工作都做了，很是赶时间 不过所幸是完成了 但是结果并不好）

　　见到题目的时候是有思路的，而且还是比较完整的。但是可惜的是在构造思路的时候并没有实际的去研究一下这个思路是不是可行的（不过所幸这个思路大体没有问题）

　　所以在开始之后就不停的遇到计划之外的事情，比如说我在定位图片上某一个点的时候，本来想的是通过找角点的方式找到那个点，但是效果并不好（事实是一个点都没找准）

　　然后又尝试去找到图片上面的矩形，但是可惜的是，图形上面的矩形也不过是对人眼来说比较清楚而已，对于代码来说完全找不到矩形在哪里。。。（实际上我觉得这个思路最大的难点就是处理145张图片中某些图片的明暗区别）

　　然后就又用上了模型匹配的方法，真的不喜欢这个算法，，，去年用`matlab`手动实现了模型匹配 结果是完全匹配所花费的时间达到了`十几秒`，，，各种优化之后才降低到了`两三秒` 但是付出的代价就是精度缺失（不过`Python`封装的那个算法是真的厉害，一秒不到就能匹配完成）

　　这样的话 第一题倒是完成了，

　　接着第二题就是确定虫道位置了，`Python`有直接能够描边的代码，，， 所以这里比较顺利，直接就得到了边缘点上的每一个点的位置（但是实际上最后发现其实它记录的每一个拐角的坐标（比如一个矩形，再大也仅仅记录四个角坐标））

　　第三题比较烧脑，主要就是`Python`似乎没有直接对点云数据进行重建的算法，这个我也是有思路的 但是想要实现比较麻烦，实际做了之后效果并不好，然后就是常用的表面重建算法并不会。。。（所以你TM参加什么比赛啊）

　　不过得到点云数据还是比较顺利的，但是重建这个部分真的很头大 

　　比赛期间还考虑了神经网络，，，但是，不会啊 [捂脸] 不过决定了要学学，因为这个真的蛮有意思的。而且 后面会用到。 

　　这次比赛给我的警醒就是我这个思路很匮乏，总不能每次都使用这样莽的算法，太莽了。主要还是源于知识不够，需要学习的还是有很多的。

　　其次就是，遇到问题先百度，倒不是说完全依赖百度，这里主要是不能做重复的工作，比如说在第二题里面，如果是手动描边，真的很花费时间以及脑力，在哪里做了一个下午研究的算法甚至不如人家一行代码速度快，何必呢。而且可以拓宽思路，不是吗？
