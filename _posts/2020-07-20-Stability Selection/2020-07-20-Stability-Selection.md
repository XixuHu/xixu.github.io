---
title: Stability Selection
category: High dimensional statistics
tags:
  - Concept and Theory
---

$$
\begin{align*}
\newcommand{\Hilbert}[1]{\mathscr{#1}}
\newcommand{\dd}{\operatorname{d}}
\newcommand{\op}{\hat}
\newcommand{\id}{\mathbf{I}}
\newcommand{\Tr}[1]{\operatorname{Tr}\left\lbrace#1\right\rbrace}
\newcommand{\realset}{\mathbb{R}}
\newcommand{\intset}{\mathbb Z }
\newcommand{\comset }{\mathbb C }
\newcommand{\innerproduct}[1]{\left\langle #1 \right\rangle}
\renewcommand{\vec}{\mathbf}
\newcommand{\spl}[1]{\langle{#1}\rangle}
\newcommand{\inner}[2]{\left\langle{#1,#2}\right\rangle}
\newcommand{\form}{\tilde}
\newcommand{\abs}[1]{\left\vert{#1}\right\vert}
\newcommand{\bra}[1]{\left\langle{#1}\right\vert }
\newcommand{\ket}[1]{\left| {#1}\right\rangle}
\newcommand{\braket}[2]{\left\langle {#1} \; \middle|\;{#2} \right\rangle }
\newcommand{\mani}{\mathcal}
\newcommand{\field}{\mathscr}
\newcommand{\Tspace}[1]{T\! {#1}}
\newcommand{\D}[2]{\frac{\d {#1}}{\d {#2} }}
\newcommand{\Partial}[2]{\frac{\partial {#1} }{\partial {#2} }}
\newcommand{\op}{\hat}
\newcommand{\uvec}{\hat}
\newcommand{\defas}{: =}
\newcommand{\isdefas}{= :}
\newcommand{\Eqn}[1]{\text{(Eqn. }\ref{#1}\text{)}}
\newcommand{\dual}{\tilde}
\newcommand{\vard}{\mathfrak{d}}
\newcommand{\vare}{\mathfrak{e}}
\newcommand{\e}{\mathrm{e}}
\newcommand{\ii}{\mathrm{i}}
\newcommand{\blue}{\color{blue}}
\newcommand{\red}{\color{red}}
\newcommand{\norm}[1]{\left\|{#1}\right\|}
\newcommand{\set}[1]{\left\lbrace{#1}\right\rbrace}
\newcommand{\sgn}{\operatorname{sgn}}
\newcommand\myeq{\stackrel{\mbox{adiabatic}}{=}}
\newcommand{\avg}[1]{\left\langle {#1} \right\rangle}
\end{align*}
$$

**正则化路径**是每个变量的系数随正则化参数变化的曲线；**稳定性路径**是当随机选取数据的一部分时，每个变量被选中的概率。对一个给定的惩罚系数$\lambda$，被选出的集合$\hat{S}^{\lambda}$是(隐式的)样本指标集的函数$I=\{1, \ldots, n\}$。我们记$\hat{S}^{\lambda}=\hat{S}^{\lambda}(I)$来表示这种依赖性。

`Def`：**入选概率**

记$I'$为$\{1, \ldots, n\}$的一个大小为$\lfloor n / 2\rfloor$无放回子指标集，对特征集的任何子集$K$来说，他的入选概率定义为
$$
\hat{\Pi}_{K}^{\lambda}=P^{*}\left\{K \subseteq \hat{S}^{\lambda}(I)\right\}
$$
选择$\lfloor n / 2\rfloor$是因为这是最接近bootstrap的采样方式，同时可以兼顾计算上的便利。(理论保证：Freedman, 1977;

Büchlmann and Yu, 2002)

## References

[1] [Stability selection]()

