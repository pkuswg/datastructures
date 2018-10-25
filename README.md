# 代码依据`数据结构与算法分析c++描述`写的
 * ## [二叉查找树](Binarytree.java)
 * ## [堆排序](heap_sort.java)
 ```text
 没什么好说的，建最大堆。采用下滤。
 ```
 * ## [插入排序](insert_sort.java)
 ```text
 O(n2)算法中比较有特点的一种：对数据有序识别很好。
 ```
 * ## [希尔排序](shell_sort.java)
   插入排序的改进，插入排序的特点是如果数据基本有序，其运行时间更快。希尔排序采用一个增量序列h1=1，h2,h3...hk。
   依次进行hk，h(k-1),h(k-2),..h1排序，共计k趟排序，每次排序数据更倾向于有序，因此最后一趟插入排序运行时间很短。
   具体每一趟排序过程是：对于hk,hk-1,hk-2...N-1(默认下标为0到N-1)中每一个值i，放到i-hk,i-2hk,i-3hk,...中正确
   的位置上。
   ```text
    堆排序与希尔排序对于循环的编写很有代表性，循环的编写应该把每次迭代的不变量放到循环体中，都要以这个基准来写条件测试表达式
   ```
  * ## [快速排序](quick_sort.java)
  ```text
  由于之前疏忽，采用三数取中值来获取随机的值的过程，不仅减少了最坏情况发生频率，实际更隐含了对边界的检查。
  在代码中我直接取第一个值，二没有检查边界，导致产生越界错误。
  ```
