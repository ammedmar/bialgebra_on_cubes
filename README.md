# Algebraic $E_\infty$-bialgebra on cubes

In this notebook we describe a natural $E_\infty$-bialgebra structure on the chains of a standard cube using the finitely presented $E_\infty$-prop of [[1]](https://arxiv.org/abs/1808.00854).

## Preliminaries
### $E_\infty$-coalgebras and $E_\infty$-bialgebras

Let $k$ be a commutative and unital ring. In this notebook we will consider $k$ to be the field with two elements, but the following definitions and statements hold in general. 

An $E_\infty$-coalgebra structure on a chain complex $C$ is a morphism of operads 

$$\mathcal E \to \big\{ \mathrm{Hom} (C, C^{\otimes m}) \big\}_{m \geq 0}$$

where $\mathcal E(0) = k$ and $\mathcal E(m)$ is a free $k[\Sigma_m]$-module with the homology of a point. Such operad is called an $E_\infty$-operad.

An $E_\infty$-bialgebra structure on a chain complex $C$ is a morphism of props

$$\mathcal P \to \big\{ \mathrm{Hom} (C^{\otimes n}, C^{\otimes m}) \big\}_{n,m \geq 0}$$

that restricted to the operad $U(\mathcal P) = \{\mathcal P(1,m)\}_{m \geq 0}$ defines an $E_\infty$-coalgebra structure on $C$.

In [[1]](https://arxiv.org/abs/1808.00854) is shown that a choice of three maps: 

$$\Delta : C \to C \otimes C$$
of degree 0,
$$\varepsilon : C \to \mathbb F_2$$
of degree 0, and
$$\ast : C \otimes C \to C$$

of degree one, define an $E_\infty$-bialgebra structure on $C$ if they satisfy for every $x,y \in C$

$$(\partial \otimes \mathrm{id} + \mathrm{id} \otimes \partial) \Delta (x) = \Delta\,(\partial(x))$$

$$\partial \varepsilon (x) = 0$$

$$\partial (x \ast y) + (\partial x) \ast y + x \ast (\partial y) 
= \varepsilon(x)y + \varepsilon(y)x$$
and 
$$(\varepsilon(x) \otimes \mathrm{id})\,\Delta(x) = x = (\mathrm{id} \otimes \varepsilon(x))\,\Delta(x)$$

$$\varepsilon(x \ast y) = 0.$$

In this notebook, we describe using this method a natural $E_\infty$-bialgebra structure on the chains of standard cubes. We remark that, using a standard technique from category theory, this defines an $E_\infty$-coalgebra structure on the chains of cubical sets.
