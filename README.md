# 8-Input-Sorting-Circuit-4-bit

This repository describes the design of a combinational sorting circuit for eight unsigned 4-bit numbers (X0..X7). The circuit takes these eight inputs and outputs the same eight numbers, but in sorted order, sorting is obtained by using theBatcher Odd - Even Mergesort Algorithm from least to greatest(Y0..Y7). The report outlines the design approach, analyzes its power consumption and worst-case propagation delay, and provides a transistor-level schematic for the core sorting element.

**Introduction**

The basic principle of Batcher’s Odd-Even Mergesort is a merge algorithm that joins two sorted sequence halves to produce a fully sorted sequence. Batcher’s Odd-Even Merge-sort is popularized as an efficient sorting method for graphics processing hardware. It’s used in parallel computing and sorting networks. Batcher’s method constructs sorting networks of size O(n(logn)2) and depth O((logn)2), where n represents the number of items to be sorted.

![image](https://github.com/Nirvan-Mishra-09/8-Input-Sorting-Circuit-4-bit/assets/127642231/52aa2329-28de-4793-be5f-5642ffc34256)
![Untitled Diagram drawio](https://github.com/Nirvan-Mishra-09/8-Input-Sorting-Circuit-4-bit/assets/127642231/b81f5593-5dde-4184-a342-7a5e6c605c56)

The above design  utilizes a series of sorting units at each stage. Each sorting unit is composed of two key components: a comparator and a swapping unit.
The **comparator unit** acts as the brain of the sorting circuit, responsible for determining the relative order of two input numbers. It takes two 4-bit unsigned numbers (A and B) as inputs and produces three outputs:

1. A greater than B (A_GT_B): logic 1 if A is greater than B, else logic 0.
2. A less than B (A_LT_B): logic 1 if A is less than B, else logic 0.
3. A equals to B (A_EQ_B): logic 1 if A equals B, else logic 0

![1](https://github.com/Nirvan-Mishra-09/8-Input-Sorting-Circuit-4-bit/assets/127642231/c4731566-7799-4779-b075-7bfedf6d6fbe)
