---
layout: post
title: "Images and Kernels of Linear Maps and Bijectivity"
author: "Kong Yao"
categories: journal
tags: [linear algebra, analysis]
image: sg1.jpg
---
This note elaborates on the relationship between the image and kernel of linear maps and the two components of bijectivity, namely injectivity and surjectivity. In a first course in linear systems theory, the following two facts are often presented as pseudo-definitions, and may not be immediately obvious nor intuitive. Below is an attempt to give more intuition to these facts using more precise mathematical terms.

***

Suppose $A$ is a linear map between two vector spaces $\mathcal{U}$ and $\mathcal{V}$, $\textit{i.e.,}$ $A: \mathcal{U} \to \mathcal{V}.$ 

$\textbf{Fact 1}$: $A$ is $\textit{surjective}$ if the image of $A$, denoted by $\textbf{Im}(A)$, is equals to $\mathcal{V}.$ 

$\textbf{Fact 2}$: $A$ is $\textit{injective}$ if the kernel of $A$, denoted by $\textbf{Ker}(A)$, is equals to the zero vector, $\\{0\\}.$ 

***

To understand Fact 1 better, we recall the definitions of an image of a linear map and surjectivity.

$\textbf{Definition 1}$: The image of a linear map $A$, denoted by $\textbf{Im}(A)$, is the set $\\{v \in \mathcal{V} \,:\, \exists\, u \in \mathcal{U} \;\;s.t.\; A(u) = v\\}.$  

$\textbf{Definition 2}$: A linear map $A : \mathcal{U} \to \mathcal{V}$ is surjective if for all $v \in \mathcal{V}$, there exists $u \in \mathcal{U}$ such that $A(u) = v$.

These two definitions look almost identical. The only difference lies in the quantifier, "for all $v \in \mathcal{V}$", which may not be true for $\textbf{Im}(A)$. In other words, if $\textbf{Im}(A)$ contains every element of the entire range $\mathcal{V}$, then surjectivity holds. 

***

For Fact 2, let's revisit the definitions of a kernel of a linear map and injectivity.

$\textbf{Definition 3}$: The kernel of a linear map $A$, denoted by $\textbf{Ker}(A)$, is the set $\\{u \in \mathcal{U}: A(u) = 0\\}.$

$\textbf{Definition 4}$: A linear map $A : \mathcal{U} \to \mathcal{V}$ is injective if for all $x,y \in \mathcal{U}$, if $A(x) = A(y)$, then $x=y$.

From the above definitions, Fact 2 appears to be less obvious. To show this, observe that since $A$ is a linear map, for any $x,y \in \mathcal{U}$,

$$A(x) = A(y) \Leftrightarrow A(x) - A(y) = 0 \Leftrightarrow A(x-y) = 0$$

This condition corresponds exactly to the definition of $\textbf{Ker}(A)$. If $\textbf{Ker}(A)$ is equals to the zero vector $\\{0\\}$, then $x-y = 0$. Hence, $x = y$ and $A$ is injective.

***

If $A$ is both surjective and injective, then $A$ is said to be $\textit{bijective}$. In that case, the inverse map $A^{-1}$ exists and is well-defined, making the expression $A^{-1}(v) = u$ admissible. 