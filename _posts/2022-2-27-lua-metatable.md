---
layout:       post
title:        Lua 元表
created:      '2022-02-27T19:17:06.154Z'
modified:     '2022-03-30T15:31:17.255Z'
author:       "xiaohao"
header-style: text
catalog:      true
tags:
    - Lua
---

# Lua 元表

## 前言

## 定义
可以通过元表来修改一个值的行为，使其在面对一个非预定义的操作时执行一个指定的操作，比如对两个table相加，可以通过定义元表中的__add元方法去定义两个table的相加。

## 原理
比如当Lua试图将两个table相加时，它会先检查两者之一是否有元表，然后检查该元表中是否有一个叫__add的字段，如果找到了该字段，就调用该字段对应的一个值，这个值也就是所谓的“元方法”，它应该是一个函数。
在新创建一个table时，是不会创建元表的。

## 元表代码
~~~ lua
local t = {}
local meta = {}
setmetatable(t, meta)
~~~

## 元方法
### 1 算术类
#### __add
加法，可以使两个值相加，可以是table加数值，也可以是table加table。

#### __mul 乘法

#### __sub 减法

#### __div 除法

#### __unm 相反数

#### __mod 取模

#### __pow 乘幂

#### __concat 描述连接操作符

### 2 关系类
#### __eq 等于
~~~ lua

~~~

#### __lt 小于

#### __le 小于等于

### 3 库定义的元方法
#### __tostring

#### __call

#### __metatable

#### __gc

### 4 访问table的元方法
#### __index

#### __newindex

## 链接
- http://dingxiaowei.cn/2017/06/18/
- [元表和闭包](http://dingxiaowei.cn/2018/10/10/)
- Lua程序设计第2版
