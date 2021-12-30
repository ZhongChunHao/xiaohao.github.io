---
layout:       post
title:        "[Unity Shader] 三 数学基础"
subtitle:     "unity shader"
created:      '2020-05-08T03:51:47.094Z'
modified:     '2020-05-23T02:35:53.014Z'
author:       "CharlesZhong"
header-style: text
catalog:      true
published:    false
tags:
    - Unity Shader
    - Shader
---

# [Unity Shader] 三 数学基础

## 1 矩阵运算
### 1.1 矩阵相乘
先了解，矩阵相乘是规定前后顺序的，也就是A矩阵乘B矩阵和B矩阵乘A矩阵是不同的，然后矩阵相乘是有条件的，比如A矩阵乘B矩阵，得到C矩阵，要求A矩阵的列和B矩阵的行是相等的，才能相乘，比如A是2行3列的矩阵，B是3行2列的矩阵，这样就能相乘，最后得到的C矩阵是2行2列的矩阵，如果A是2行2列的，B是3行3列的，那就不能相乘。

$$
\begin{pmatrix}
   a11 & a12 \\
   a21 & a22
\end{pmatrix}
$$

### 1.2 矩阵置反

### 1.3 点积和叉积

## 2 资料
书籍
- 《大学离散数学》
- 《Unity Shader入门精要》
