---
title: Partitions, mod 6.
description: a nice problem
tags: math partitions
---

Prove that the number of partitions of $n$ in which no part appears exactly once equals the number of partitions of $n$ into parts not congruent to $\pm 1$ mod 6.

*Proof*. First, we write out the generating functions both for the number of partitions where no part appears exactly once as well as for the number of partitions where no part is congruent to $\pm 1$ mod 6.

The first generating function would be

<div style="object-fit:cover">\begin{equation}\prod_{k=1}^{\infty}\left(\frac{1}{1-x^k} - x^k\right),\end{equation}</div>

as we are simply removing the term corresponding to using exactly one part of a given size.

The second generating function would be

<div style="object-fit:cover">\begin{equation}\left(\frac{1}{1-x^2}\right)\left(\frac{1}{1-x^3}\right)\left(\frac{1}{1-x^4}\right)\left(\frac{1}{1-x^6}\right)\cdots\end{equation}</div>

as we skip $1, 5, 7, 11, \ldots$.

Let’s rewrite the generating function where no partition appears more then once. The $k$th factor combines to give $\frac{x^{2k}-x^k+1}{1-x^k}$, for $k\ge 1$. Since

<div style="object-fit:cover">\begin{equation}x^{2k}-x^k+1 = \frac{1+x^{3k}}{1+x^k}\end{equation}</div>

by sum of cubes, we can rewrite this generating function into

<div style="object-fit:cover">\begin{equation}\prod_{k=1}^{\infty} \frac{1 + x^{3k}}{(1-x^k)(1+x^k)}.\end{equation}</div>

This cancels out to

<div style="object-fit:cover">\begin{equation}\frac{1}{\left(1-x\right)\left(1+x\right)}\frac{1}{\left(1-x^2\right)\left(1+x^2\right)}\frac{1}{\left(1-x^3\right)}\cdots,\end{equation}</div>

which can be further simplified to

<div style="object-fit:cover">\begin{equation}\frac{1}{\left(1-x^2\right)}\frac{1}{\left(1-x^4\right)}\frac{1}{\left(1-x^3\right)}\frac{1}{\left(1-x^6\right)}\cdots.\end{equation}</div>

The only exponents remaining are either multiples of 3 or even numbers not divisible by 3. By Bézout’s identity, we are left with x to powers not congruent to $\pm 1$ mod 6.

Therefore, the generating functions for the number of partitions of $n$ in which no part appears exactly once and the number of partitions of $n$ into parts not congruent to $\pm1$ mod 6 are equal.
