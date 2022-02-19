---
layout: post
title: Graph Theory
datetime: 2022-02-15
category: math_notes
state: show
---
# 图
## 你需要知道的符号
$\binom{V}{k}:\{S\subset V| \left| S\right|=k \}$
$[n]:\{1,2,3...n\}$
## 图的定义
图是有一个点集V和边集E组成的有序对(V,E)
且$E\subset V^2$
## 图(无标号)的同态
若图$G_1(V_1,E_1)$与$G_2(V_2,E_2)$之间存在一一映射$f:V_1 \rightarrow V_2$
使得$xy\in E_1$当且仅当$f(x)f(y)\in E_2$,则称$G_1 \cong G_2$
#### 无向图
  $(u,v)\in E \Rightarrow (v,u)\in E$
#### 多重图(multigraph)
$E$ is a multiset of $\binom{V}{1} \cup \binom{V}{2}$
#### 超图
$E \subset 2^{V}$
#### k完全图
$([n],\binom{[n]}{2})$
#### 环
$([n],{(i,i+1)|i=1,2,3...n-1})$
#### 二分图(Bipartite Graph)
$V=A\cup B ,A\cap B=\Phi,E\subset (AxB)\cup(BxA)$
#### r分图(r-partite Graph)
$(\cup_{i=1}^{r}A_i,{xy:x\subset A_i,y\subset A_j,i\neq j})$
#### Peterson Graph
$(\binom{[5]}{2}),\{ \{ S,T \} : S,T\in \binom{[5]}{2} , S\cap T=\Phi \}$
#### Kneser Graph
$(\binom{[n]}{k}),\{ \{ S,T \} : S,T\in \binom{[n]}{k} , S\cap T=\Phi \}$
#### n维超立方体的同态
$(2^{[n]},\{ \{ S,T \} :S,T \in 2^{|n|},|S \Delta T|=1 \} )$
## 图的参数
#### 平凡的
$G$ is non-trival when $|E|\neq 0$
#### 图的阶(order)
$|G|$ 有$|G|=|V|$
#### 图的大小(size)
$||G||$,有$||G||=|E|$
#### 图的领域(neighborhood)
$S\subset V$,S的领域写作$N(S)$为与S直接相连的点。特殊的，
$N( \{ v \} )$也写作$N(v)$
#### 邻接矩阵(adjacency matrix)
$G(V,E)$,$A$是个$|G|\times |G|$的矩阵，且当$ij\in E$时,$A_{ij}=1$,
否则$A_{ij}=0$,我们称$A$为$G$的邻接矩阵
#### 度数(degree)
$d(v)$表示与v相连的点的数量
#### 叶子(leaf)节点与孤立点(isolated)
$d(v)=0$,孤立结点
$d(v)=1$,叶子结点
#### 度数序列
$\{ d_n \}$
#### 最大度与最小度
$\Delta (G)$表示最大的度数和$\delta (G)$最小的度数
#### 平均度数
$d(G)=\frac{\Sigma_{v \in V} d(v)}{|G|}$
#### 握手定理(Handshake Lemma)
$2|E|=\Sigma_{v\in V}d(v)$

$Proof. Quite Easy $
## 子图(Subgraphs)
#### 定义
$G_1(V_1,E_1)$是$G(V,E)$的子图，写作$G_1 \subset G_2$,
$G_1 \subset G_2 \Leftrightarrow V_1\subset V 且E_1 \subset E$
### Referance
[MariaAxenovich_KIT_2020GraphTheoryLectureNotes](/files/MariaAxenovich_KIT_2020GraphTheoryLectureNotes.pdf)