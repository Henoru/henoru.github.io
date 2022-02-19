---
layout: post
title: Group Theory one
datetime: 2022-02-15
category: math_notes
state: show
---
### 二元运算
#### 定义
$$ *:G^2 \rightarrow G$$
一个有序数对到一个数的映射被称作二元运算
### 群
#### 定义
一个集合与定义在集合上满足下列条件的运算
(1).$\exist 1\in G,s.t.\forall x\in G\quad 1*x=x*1=x$，既存在单位元
(2).$\forall x,y,z\in G,(x*y)*z=x*(y*z)$，既满足结合率
(3).$\forall x\in G,\exist y \in G,s.t.\quad x*y=y*x=1$

#### eg.
##### 克莱因四元群
$G=\{ I,a,b,c\} $
$a*a=1\quad b*b=1 \quad c*c=1$
$a*b=b*a=c$
$b*c=c*b=a$
$c*a=a*c=b$
容易验证，上述四元集合及其运算$$*$$满足群的定义

##### 等边三角形变换群
tips：集合的元素为变换(函数)
1.本身(ABC-ABC)
2.顺时针120(ABC-CAB)
3.逆时针120(ABC-BCA)
4.翻转(ABC-ACB)
5.翻转逆时针120(ABC-CBA)
6.翻转顺时针120(ABC-BAC)
经过验证，满足结合律且存在逆元，为群

### 群的部分性质及其证明
#### 单位元唯一
$$假设a,b都是单位元$$
$$有a*b=a=b$$
$$Q.E.D.$$

#### 逆元唯一
$$假设b,c均为a的逆元$$
$$ bac=1*c=c,bac=b*(ac)=b$$
$$ b=c$$

#### 群方程一定有解
$$ax=b$$
$$由于一定存在逆元有x=a^{-1}b$$
tips:由于群不一定满足交换律，$a^{-1}b\neq ba^{-1}$

待续