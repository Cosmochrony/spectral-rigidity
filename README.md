This repository contains the source of the **Spectral Gram Rigidity** Cosmochrony paper  
*Spectral Gram Rigidity and Structural Selection among Finite SU(2) Subgroups*.

This work constitutes **Step C of the spectral admissibility programme**.  
It establishes a structural rigidity theorem showing that the geometry of
neutral generating sets in SU(2) uniquely constrains the underlying group.

While **spectral admissibility** bounds the amplitude of individual modes
and **spectral capacity** aggregates admissible amplitudes across
representation sectors, the present work shows that the **Gram geometry
of neutral generators rigidly determines the group type**.

## Core Result

Let $S=S^{-1}$ be a **symmetric neutral generating set** for an irreducible
representation $\rho : G \to SU(2)$ satisfying

$\chi_\rho(s)=0 \quad \forall s\in S$.

Each generator can be written

$\rho(s)= i\,(\mathbf u_s\cdot \sigma)$

for a unit axis $\mathbf u_s\in S^2$.
The **Gram matrix**

$G_{st}=\mathbf u_s\cdot \mathbf u_t$

satisfies the exact identity

$G_{st}=-\tfrac12\,\chi_\rho(st)$.

Thus the full axis geometry of the generating set is encoded
directly in the character table of the representation.

## Second-Moment Tensor

Define the **second-moment tensor**

$M=\sum_{s\in S_+}\mathbf u_s\mathbf u_s^{\mathsf T}$.

Its spectral structure determines whether the generating axes
are isotropically distributed.

For binary dihedral groups $\mathrm{Dic}_n$ the eigenvalues are

$\mathrm{spec}(M)=
\begin{cases}
(n,n,0) & n\ \text{odd}\\
(n,n+2,0) & n\ \text{even}
\end{cases}$

showing that

$M\not\propto I \qquad (n\ge3)$.

Hence dihedral subgroups are **spectrally anisotropic**.

## Orthogonal Block Lemma

If the Gram matrix satisfies

$G_{st}=0 \quad \forall s,t\in S,\; t\neq s^{\pm1}$

then the axes form three mutually orthogonal directions in $\mathbb{R}^3$.

Closure of the corresponding generators implies

$\rho(G)=Q_8$.

Thus orthogonal Gram structure rigidly forces the quaternion group.

## Exclusion of the Binary Tetrahedral Case

For the binary tetrahedral group $2T$ the traceless elements are

$\{\pm i,\pm j,\pm k\}$,

which generate only $Q_8$ rather than the full group.

Therefore **no symmetric neutral generating set exists for $2T$**.

The projective case $A_4$ is consequently excluded from the admissible
classification.

## Main Rigidity Theorem

Let $S=S^{-1}$ be a symmetric neutral generating set for
$\rho:G\to SU(2)$ irreducible.

Exactly three structural regimes occur:

1. **Anisotropic second moment**

   $M\not\propto I$

   $\Rightarrow\ \bar\rho(G)=D_n,\; n\ge3$

2. **Isotropic with orthogonal Gram**

   $M\propto I,\quad G_{st}\in\{0,\pm1\}$

   $\Rightarrow\ \rho(G)=Q_8$

3. **Isotropic with non-trivial Gram angles**

   $\exists s,t:\;G_{st}\notin\{0,\pm1\}$

   $\Rightarrow\ \rho(G)\in\{2O,2I\}$

Thus the Gram geometry rigidly separates

$Q_8,\quad 2O,\quad 2I$

from all other finite subgroups of $SU(2)$.

## Relation to Klein's Classification

Klein's classification of finite $SU(2)$ subgroups gives

$\{\mathbb Z_n,\ \mathrm{Dic}_n,\ 2T,\ 2O,\ 2I\}$.

Combining the rigidity theorem with the exclusion of $2T$
yields the **admissible structural list**

$Q_8,\quad \mathrm{Dic}_n\ (n\ge3),\quad 2O,\quad 2I$.

Among isotropic configurations only

$Q_8,\ 2O,\ 2I$

remain.

## Conceptual Structure

Spectral Gram Rigidity integrates:

1. Character-theoretic reconstruction of generator geometry
2. Gram matrices of neutral generators
3. Second-moment isotropy analysis
4. Quaternionic closure constraints
5. Klein classification of finite $SU(2)$ subgroups

Together these yield a **rigidity principle linking spectral data,
representation theory, and generator geometry**.

## Status

This framework is:

- representation-theoretic
- fully analytic (no numerical assumptions)
- consistent with spectral admissibility and spectral capacity
- structurally complete for finite $SU(2)$ subgroups

It does not assume:

- spacetime geometry
- quantum field dynamics
- microscopic physical interpretation beyond relational constraints.

## Repository Structure
```
paper/
├── pdf/ # Compiled Spectral Gram Rigidity PDF
├── tex/ # LaTeX sources
└── README.md
```

## Citation

If you reference this work, please cite:

> J. Beau, *Spectral Gram Rigidity and Structural Selection among Finite SU(2) Subgroups*, Zenodo, 2026.

## Acknowledgements

Portions of the formal derivations, consistency checks, and editorial refinement
benefited from iterative interactions with large language models used as analytical
assistants.  
All theoretical results and interpretations remain the sole responsibility of the author.

## Contributions

This repository is intended as a research reference.

Critical feedback, mathematical scrutiny, and independent analyses of
finite-group Gram structures are welcome.  
Please open an issue to discuss conceptual points, technical details,
or possible extensions.
