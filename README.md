# isotropic-subspaces-for-skewforms
Computes d(F, n, k) for prime-order fields (see 'Isotropic Subspaces for Skewforms and Maximal Abelian Subgroups of p-Groups', Buhler, Gupta, Harris, 1987).

You will need to specify the dimension dim_W of the subspaces you want to test against the k bilinear forms. For small values, there will only be a few. d(F, n, k) is the largest value of dim_W such that the number of collections of k bilinear forms tested aligns with the number of those which have a dim_W-dimensional isotropic subspace.

## Overview
Let **F** be a finite field of prime order, and let $n$ and $k$ be positive integers. Let $V$ be an $n$-dimensional vector space over **F** and $\alpha = {\alpha_1, ..., \alpha_k}$ be a collection of $k$ skewforms (i.e. alternating bilinear forms) on $V$. A subspace $W$ of $V$ is said to be isotropic for $\alpha$ if it is isotropic for every $\alpha_i$. Let $m(\alpha)$ denote the dimension of the largest isotropic subspace for $\alpha$. Then $d($**F**$, n, k)$ is defined to be the minimum value of $m(\alpha)$ as $\alpha$ ranges over all collections of $k$ skewforms on $V$.
