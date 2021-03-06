学习笔记

时间、空间复杂度分析是数据结构和算法中非常重要的知识点。

> 复杂度也叫渐进复杂度，包括时间复杂度和空间复杂度，用来分析算法执行效率与数据规模之间的增长关系，可以粗略地表示，越高阶复杂度的算法，执行效率越低。

## 什么是数据结构？什么是算法？

广义来讲，数据结构就是指一组数据的存储结构。算法就是操作数据的一组方法。数据结构和算法是相辅相成的，数据结构服务于算法，算法要作用在特定的数据结构之上。

20个最常用的最基础的数据结构和算法：
10个数据结构: 数组，链表，栈，队列，散列表，二叉树，堆，跳表，图，Trie树
10个算法： 递归，排序，二分查找，搜索，哈希算法，贪心算法，分治算法，回溯算法，动态规划，字符串匹配算法

## 为什么需要复杂度分析？

数据结构和算法本身解决的是“快”和“省”的问题，即如何让代码运行得更快，如何让代码更省存储空间，复杂度分析就是用来衡量算法的执行效率。

## 大 O 复杂度表示法

所有代码的执行时间 T(n) 与每行代码的执行次数 n 成正比。

> T(n) = O(f(n))

## 时间复杂度分析

> 大 O 时间复杂度实际上并不具体表示代码真正的执行时间，而是表示代码执行时间随数据规模增长的变化趋势，所以，也叫作渐进时间复杂度（asymptotic time complexity），简称时间复杂度

![时间复杂度](https://cdn.jsdelivr.net/gh/stupid-yu/cdn/img/algorithm/O-demo.jpg)

三个实用时间复杂度分析方法

+ 只关注循环执行次数最多的一段代码
+ 加法法则：总复杂度等于量级最大的那段代码的复杂度
+ 乘法法则：嵌套代码的复杂度等于嵌套内外代码复杂度的乘积

## 空间复杂度分析

> 空间复杂度全称就是渐进空间复杂度（asymptotic space complexity），表示算法的存储空间与数据规模之间的增长关系。

我们常见的空间复杂度就是 O(1)、O(n)、O(n²)，像 O(logn)、O(nlogn) 这样的对数阶复杂度平时都用不到。