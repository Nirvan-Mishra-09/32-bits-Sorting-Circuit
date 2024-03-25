# 8-Input-Sorting-Circuit-4-bit

This repository describes the design of a combinational sorting circuit for eight unsigned 4-bit numbers (X0..X7). The circuit takes these eight inputs and outputs the same eight numbers, but in sorted order, sorting is obtained by using theBatcher Odd - Even Mergesort Algorithm from least to greatest(Y0..Y7). The report outlines the design approach, analyzes its power consumption and worst-case propagation delay, and provides a transistor-level schematic for the core sorting element.

**Introduction**

The basic principle of Batcher’s Odd-Even Mergesort is a merge algorithm that joins two sorted sequence halves to produce a fully sorted sequence. Batcher’s Odd-Even Merge-sort is popularized as an efficient sorting method for graphics processing hardware. It’s used in parallel computing and sorting networks. Batcher’s method constructs sorting networks of size O(n(logn)2) and depth O((logn)2), where n represents the number of items to be sorted.

![image](https://github.com/Nirvan-Mishra-09/8-Input-Sorting-Circuit-4-bit/assets/127642231/52aa2329-28de-4793-be5f-5642ffc34256)

