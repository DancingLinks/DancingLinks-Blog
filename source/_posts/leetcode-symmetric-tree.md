---
title: leetcode symmetric-tree
date: 2020-03-04 18:48:23
tags:
    - 二叉树
---

## 传送门

https://leetcode-cn.com/problems/symmetric-tree/

## 大意

给定一个二叉树，检查它是否是镜像对称的。

## 思路

首先题目要求是否镜像，如果一个树的左子树与右子树镜像对称，那么这个树是对称的。那么很容易可以想到，可以抽象成以下过程：

1. 比较A、B是否相同
2. 比较A的左节点、B的右节点是否相同
3. 比较A的右节点、B的左节点是否相同

所以代码很容易就实现了，初始情况下可以传入root节点与自身比较。

## 代码

``` go
/**
 * Definition for a binary tree node.
 * type TreeNode struct {
 *     Val int
 *     Left *TreeNode
 *     Right *TreeNode
 * }
 */

func check(a, b *TreeNode) bool {
    if a == nil && b == nil {
        return true
    }
    if a == nil || b == nil {
        return false
    }
    return a.Val == b.Val && check(a.Left, b.Right) && check(a.Right, b.Left)
}

func isSymmetric(root *TreeNode) bool {
    return check(root, root)
}

```
