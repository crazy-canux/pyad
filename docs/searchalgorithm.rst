.. _searchalgorithm:

search algorithm
================

七大查找算法


linear search/线性查找
-----------------------

线性查找又叫顺序查找(sequential search).

从第一个到最后一个和要查找的内容比较.

* 时间复杂度

    O(n)

* 空间复杂度


binary search/二分查找
----------------------

二分查找又叫折半查找.只能用于有序序列。

设置三个下标，min=0, max=array.length - 1, mid = (min+max)/2。
然后用要查找的关键值key和mid下标的元素比较。
如果key比array[mid]大，那么将数组一分为二，min变为mid+1,mid重新计算。
如果key比array[mid]小，那么数组一分为二，max变为mid-1,mid重新计算。
如果key==array[mid]那么找到了。
如果min>=max那么没有找到。
依次类推，每次将数组一分为二。

* 时间复杂度

* 空间复杂度


interpolation search/插值查找
-----------------------------

插值查找是二分查找的优化版，同样只能用于有序序列。

核心是计算公式:  (key-array[min]) / (array[max] - array[min])

mid = min + (max-min) * (key-array[min]) / (array[max]-array[min])

* 时间复杂度

* 空间复杂度


fibonacci search/斐波拉切查找
-----------------------------

只能用于有序序列.和插值/二分 策略一样，通过分割区间缩小范围.

* 时间复杂度

* 空间复杂度


tb search/树表查找
------------------


block search/分块查找
---------------------


hash search/哈希查找
--------------------

