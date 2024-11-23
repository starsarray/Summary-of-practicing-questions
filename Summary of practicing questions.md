# 目录

[动态规划](#动态规划)

​	[入门DP](#入门DP)

​	[网格图DP](#网格图DP)

# 动态规划

动态规划题目的特点：

​	问题的优化解包含了子问题的优化解，求解过程中很多子问题需要进行多次使用。

步骤：

1. 把题目结果转换成子问题的结果
2. 写出状态转移方程
3. 设置初始值和边界
4. 确定计算顺序求解

***

## 入门DP

问题的状态都是**线性**的

当前状态结果与某两个状态的结果有关

若是与前两次的状态有关，则只需使用两个变量保存这两个状态

其他情况用一维数组就可解决

***

## 网格图DP

问题的状态都是**网格型**

当前状态结果与上一行（和这一行）的多个状态结果有关

若是与紧挨着的两个状态结果(比如上一行这一列和这一行左边一列）有关，则只需使用一维数组保存这两个状态（这一行左边一列前一次计算出来了归到数组左边，上一行这一列在数组当前位置，然后计算后覆盖当前位置的状态结果）

比较难的一般都需要（多个）二维数组解决

***

## 背包

问题的状态**无序**，但加以**限制**

**![416.分割等和子集1](https://code-thinking-1253855093.file.myqcloud.com/pics/20210117171307407.png)**

### 0-1背包

每个物品只能选择一次



### 完全背包

物品可以重复选，无个数限制



### 多重背包

物品可以重复选，有个数限制



### 分组背包

同一组内的物品至多/恰好选一个