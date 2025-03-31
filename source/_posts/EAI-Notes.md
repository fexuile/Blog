---
title: EAI Notes
date: 2025-03-31 16:14:37
tags:
- EAI

---

## Force Closure
$F=[F_1, F_2, \dots, F_j], j = m \times k$，其中$m$是接触点个数，$k$是摩擦锥的选取代表向量个数。

F每一个列向量都有3行或6行，表示2D/3D的情况，要考虑关于质心的转动，所以需要多带一个（一些）力矩的参数。

## GraspNet-1Billion
数据集之中在$\mu = 1$到$\mu = 0.1$这一段之中能够得到的$\text{force closure}$是包含关系的，所以我们尽可能选取一个比较小的$\mu$，得到比较稳妥的抓取方式。