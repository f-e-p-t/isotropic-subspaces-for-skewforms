# isotropic-subspaces-for-skewforms
This is a computational approach to evaluating the function $d($**F**$, n, k)$ discussed in *Isotropic Subspaces for Skewforms and Maximal Abelian Subgroups of p-Groups*, Buhler, Gupta, Harris, 1987 ([read online](https://www.sciencedirect.com/science/article/pii/0021869387901384)).

## Definitions and Overview
Let **F** be a field, and let $n$ and $k$ be positive integers. Let $V$ be an $n$-dimensional vector space over **F** and $\alpha = {\alpha_1, ..., \alpha_k}$ be a collection of $k$ skewforms (i.e. alternating bilinear forms) on $V$. A subspace $ W\subseteq V$ is isotropic for $\alpha$ if it is isotropic for every $\alpha_i$. Let $m(\alpha)$ denote the dimension of the largest isotropic subspace for $\alpha$. Then $d($**F**$, n, k)$ is the minimum value of $m(\alpha)$ as $\alpha$ ranges over all collections of $k$ skewforms on $V$.
Buhler, Gupta and Harris' 1987 paper finds an upper bound on $d($**F**$, n, k)$ when Char(**F**)$\neq$2. The Python program in this repo calculates $d($**F**$, n, k)$ for fields **F** of prime order, including order 2.

## Usage
Set **F**, $n$ and $k$ by changing the variables at the top of the Python file. The last variable is dim_W. The program will report the number of collections $\alpha$ of $k$ skewforms that admit an isotropic subspace of dimension dim_W.
### What do the Results Mean?
- Every collection of skewforms admits an isotropic subspace of dimension dim_W: $d($**F**$, n, k)\geq dim_W$
- At least one collection of skewforms did not admit a subspace of dimension dim_W: $d($**F**$, n, k) < dim_W$
