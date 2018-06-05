---
layout: post
title: Counting selections with replacement
---

![_config.yml]({{ site.baseurl }}/images/WechatIMG57.jpeg)

You can refer to the origin blog [here](https://www.johndcook.com/blog/select_with_replacement/). 

从一个大小为n的元素集中采样k。对于无重复的情况，有(n, k)种情况，这也是组合数的定义。
对于有重复的情况，即同一个元素可以被多次取样，有(n+k-1, k)种情况。下面来简单证明这个问题：

这个问题等价于将k个无区别的球放到n个有区别的盒子中的问题。比如n=3，k=4的情况。
|\*||\*\*\*|
注意到前后两个隔板是固定的，所以需要从2个隔板+4个球中选取出四个球的位置，即(6, 4)。
