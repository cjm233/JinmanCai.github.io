---
layout: post
lang: en
title: "Baryon Operators, Topological Solitons, and Continuum Thresholds in Small-T² QCD: Research Progress and Limits of the Proof"
date: 2026-11-02
permalink: /posts/2026/11/qcd-t2-baryon-threshold/
excerpt: "Starting from transverse zero modes of four-dimensional QCD with baryon magnetic flux, we study lowest-dimension baryon operators, non-Abelian bosonization, center twists, and spectral thresholds, carefully distinguishing established results from open problems."
tags:
  - QCD
  - compactification
  - baryon
  - WZW
  - sine-Gordon
  - spectral-density
math: true
---


> **Research note (revised November 4, 2026).** This article documents an ongoing analytical research program; it does not claim to have established the lowest baryon spectrum of the original four-dimensional QCD theory. We label the strength of each result as **[Literature]**, **[Derived]**, **[Conditional]**, or **[Open]**. Operator formulas follow the normalization, chirality, and background-gauge conventions specified here.

## Abstract

Consider $$SU(3)$$ QCD with two massless quark flavors on

$$
\mathbb R^{1,1}\times T^2,
\qquad N_c=3,\quad N_f=2,\quad L\Lambda_{\rm QCD}\ll1
$$

with compatible color 't Hooft flux and baryon-number magnetic flux. Earlier studies established the relation between the four-dimensional background, two-dimensional Dirac zero modes, and the center-vortex effective theory. Here we organize the following additional results:

1. A complete classification of lowest-dimension, derivative-free $$B=1$$ operators in the two-dimensional zero-mode sector into two chiral doublets;
2. The construction of a four-dimensional point-split baryon source with a nonzero tree-level zero-mode projection, including a careful treatment of its local derivative expansion;
3. The separation of the leading local $$U(2)_1$$ WZW action into a sine-Gordon singlet sector and an $$SU(2)_1$$ flavor sector;
4. The identification of $$B=1$$ with a $$6\pi$$ winding of $$\eta'$$ and the determination of the lowest conformal weight in the **standard center-twisted model**;
5. The conditional derivation of the spectral-threshold exponent $$\alpha=-1/2$$, assuming a nonvanishing one-soliton form factor, factorization, and no dangerous defect interactions;
6. An assessment of defect RG, symmetry-compatible counterexamples involving core degrees of freedom, and the outstanding four-dimensional microscopic matching problem.

**Main result (conditional):**

$$
\boxed{\rho_B^{(1)}(s)\ \sim\ A_B\,
\Theta(s-M_B^2)(s-M_B^2)^{-1/2}}
$$

This is the **leading one-soliton continuum contribution in the minimal factorized defect model**, not an unconditional theorem about the lowest spectrum of the complete four-dimensional QCD theory.

---

## Contents

1. [Research objective and logical chain](#section-1)
2. [Four-dimensional flux compactification and two-dimensional zero modes](#section-2)
3. [Classification of the lowest-dimension two-dimensional baryon operators](#section-3)
4. [Four-dimensional baryon sources and point-splitting matching](#section-4)
5. [Non-Abelian bosonization and local factorization](#section-5)
6. [Topological baryon charge and center twist](#section-6)
7. [One-soliton threshold spectral density](#section-7)
8. [RG stability, uniqueness, and microscopic obstructions](#section-8)
9. [Scope of the results and next questions](#section-9)
10. [Appendix A: Transverse wavefunctions and the Wronskian](#appendix-a)
11. [Appendix B: Decomposition of the WZW kinetic term and three-form](#appendix-b)
12. [Appendix C: Classical kink and fluctuation spectrum](#appendix-c)
13. [Appendix D: Finite-volume spectrum of the center-twisted sector](#appendix-d)
14. [Appendix E: Phase-space derivation of the spectral density](#appendix-e)
15. [References](#references)

<a id="section-1"></a>

## 1. Research Objective and Logical Chain

The sequence of implications we aim to establish is

$$
\begin{gathered}
\text{4D QCD + background flux}
\ \longrightarrow\ \text{2D quark zero modes}
\\
\longrightarrow\ \text{baryon interpolating operators}
\ \longrightarrow\ U(2)_1\text{ WZW}
\\
\longrightarrow\ S_{\rm SG}[\eta']+S_{SU(2)_1}[g]
\\
\longrightarrow\ B=1\text{ winding + flavor gluing}
\\
\overset{\text{minimal-defect assumption}}{\dashrightarrow}
\text{one soliton + center-twisted flavor channel}
\\
\longrightarrow\ h_{\rm flavor}=\frac14
\ \longrightarrow\ \alpha=-\frac12.
\end{gathered}
$$

**Crucial caveat:** The passage from global constraints in the $$B=1$$ sector to the minimal defect fixed point **without additional core degrees of freedom** remains the most important **unproven dynamical step**. Internal consistency of the two-dimensional model cannot substitute for microscopic matching.

**Notation:** $$L$$ is the transverse $$T^2$$ size; $$R$$ is the circumference of the remaining spatial direction when it is compactified further; and $$M_B$$ is the physical mass of the lowest candidate soliton, which should not be confused with the classical small-fluctuation mass.

<a id="section-2"></a>

## 2. Four-Dimensional Flux Compactification and Two-Dimensional Zero Modes [Literature]

Write the four-dimensional coordinates as $$X=(x,y)$$, with $$x\in\mathbb R^{1,1}$$ and $$y=(x_3,x_4)\in T^2$$. In the background with one unit of baryon magnetic flux,

$$
\int_{T^2}F_B=2\pi.
$$

The color twist and baryon flux together lead to an allowed zero mode of the transverse Dirac operator, yielding one two-dimensional Dirac field per flavor. Nonzero transverse excitations have a characteristic energy of $$O(1/L)$$ [1,2].

The four-dimensional quark field admits an expansion

$$
\boxed{
q_f^{aA}(x,y)
=v^a(y)\bigl[\xi_R^A\chi_{f,R}(x)
+\xi_L^A\chi_{f,L}(x)\bigr]
+q_{f,H}^{aA}(x,y).}
$$

Here $$a=1,2,3$$ is the color index and $$A$$ is a four-dimensional Dirac index. The transverse color wavefunction is $$v^a(y)$$, while $$\xi_{R,L}$$ are fixed spinor embeddings. The two-dimensional Grassmann fields $$\chi_{f,R/L}(x)$$ have **no independent color index**. A convenient normalization is

$$
\int_{T^2}d^2y\sum_{a=1}^3|v^a(y)|^2=1.
$$

Consequently, the low-energy flavor spaces are

$$
U_R=\mathrm{span}\{\chi_{u,R},\chi_{d,R}\}
\simeq\mathbf{2}_R,
\qquad
U_L\simeq\mathbf{2}_L.
$$

**Conclusion:** The compactified microscopic background supports the construction of two-dimensional low-energy fields. However, a gap for nonzero KK modes around the vacuum background does **not** establish the absence of additional low-energy states in the interacting baryon core.

<a id="section-3"></a>

## 3. Classification of Lowest-Dimension Two-Dimensional Baryon Operators [Derived]

### 3.1 Classification from Grassmann Anticommutation

Consider derivative-free $$B=1$$ operators composed of three two-dimensional zero-mode fermion fields, with classical dimension $$\Delta_{\rm UV}=3/2$$. Their antisymmetric Grassmann products belong to

$$
\Lambda^3(U_R\oplus U_L)
=\Lambda^3U_R
\oplus(\Lambda^2U_R\otimes U_L)
\oplus(U_R\otimes\Lambda^2U_L)
\oplus\Lambda^3U_L.
$$

Since $$\dim U_R=\dim U_L=2$$,

$$
\Lambda^3U_R=\Lambda^3U_L=0,
\qquad \Lambda^2\mathbf{2}=\mathbf{1}.
$$

It follows that

$$
\boxed{
\Lambda^3(\mathbf2_R\oplus\mathbf2_L)
=(\mathbf1_R,\mathbf2_L)\oplus(\mathbf2_R,\mathbf1_L).}
$$

The $$RRR$$ and $$LLL$$ combinations therefore vanish; only the $$RRL$$ and $$LLR$$ types survive at this dimension. With $$\epsilon^{ud}=1$$, define

$$
\boxed{
\begin{aligned}
\mathcal B_R^h
&=\frac12\epsilon^{fg}
:\!\chi_{f,R}\chi_{g,R}\chi_{h,L}\!:,\\
\mathcal B_L^h
&=\frac12\epsilon^{fg}
:\!\chi_{f,L}\chi_{g,L}\chi_{h,R}\!:.
\end{aligned}}
$$

For example, $$\mathcal B_R^u=:\!\chi_{u,R}\chi_{d,R}\chi_{u,L}\!:$$ . Both types transform as $$I=1/2$$ doublets under the diagonal $$SU(2)_V$$ subgroup, with no additional $$I=3/2$$ component.

### 3.2 Lorentz Labels Versus Chiral Flavor Representations

Choose the two-dimensional Lorentz weights $$s(\chi_R)=+1/2$$ and $$s(\chi_L)=-1/2$$. Then

$$
\begin{aligned}
s(\mathcal B_R)&=+\frac12+\frac12-\frac12=+\frac12,\\
s(\mathcal B_L)&=-\frac12-\frac12+\frac12=-\frac12.
\end{aligned}
$$

This explains the subscripts $$R$$ and $$L$$ on the composite operators. By contrast, antisymmetrically contracting the flavor indices of two right-handed fields produces an $$SU(2)_R$$ singlet, so

$$
\mathcal B_R\sim(\mathbf1_R,\mathbf2_L),\qquad
\mathcal B_L\sim(\mathbf2_R,\mathbf1_L).
$$

**Scope:** The statement that there are exactly two types applies **only to derivative-free, lowest-classical-dimension operators built from the two-dimensional zero modes**. It must not be extended to claim that there are only two baryon interpolating operators in the full four-dimensional theory.

<a id="section-4"></a>

## 4. Four-Dimensional Baryon Sources and Point-Splitting Matching [Derived]

### 4.1 Why Does the Tree-Level Projection of a Local Three-Quark Source Vanish?

Consider a generic local four-dimensional baryon source, suppressing its Dirac tensor:

$$
\mathcal J_{\rm loc}(x,y)
=\epsilon_{abc}\,q^a(x,y)q^b(x,y)q^c(x,y).
$$

When all three quarks are projected onto the same transverse zero-mode wavefunction, the color factor is

$$
\boxed{
\epsilon_{abc}v^a(y)v^b(y)v^c(y)
=\det[v(y),v(y),v(y)]=0.}
$$

Thus, the tree-level projection of a **local three-quark source without transverse derivatives** onto three zero modes vanishes. This does not imply that its all-order quantum matching coefficient vanishes, nor that the two-dimensional $$\mathcal B_{R,L}$$ operators do not exist.

### 4.2 Wilson-Line-Dressed Point-Split Sources

Choose three positions $$y_i$$ on the transverse $$T^2$$ and a common base point $$y_0$$. Define

$$
\widehat q_f(x;y_i,y_0)
=W(y_0,y_i)q_f(x,y_i).
$$

Here $$W$$ parallel-transports color and background gauge indices along a specified path. The resulting four-dimensional Dirac-spinor-valued source is

$$
\boxed{
\begin{aligned}
\mathcal J_{h,\rm ps}^{A}
={}&\frac12\epsilon_{abc}\epsilon^{fg}
\bigl[\widehat q_f^{aT}(x;y_1)
C_4\gamma_3\widehat q_g^b(x;y_2)\bigr]
\widehat q_h^{cA}(x;y_3).
\end{aligned}}
$$

It is invariant under color gauge transformations; as an operator carrying total $$B=1$$, it remains charged and **gauge-covariant**, rather than invariant, under external $$U(1)_B$$ background-gauge transformations. Inserting the zero-mode expansion gives

$$
\boxed{
P_0\mathcal J_{h,\rm ps}^{A}
=D_{\rm ps}(y_1,y_2,y_3;y_0)
\bigl[\xi_R^A\mathcal B_R^h
+\xi_L^A\mathcal B_L^h\bigr],}
$$

The overall phase depends on the Dirac basis and the path conventions, and

$$
D_{\rm ps}
=\epsilon_{abc}
\widehat v^a(y_1)\widehat v^b(y_2)\widehat v^c(y_3).
$$

Therefore, if the three parallel-transported color vectors are linearly independent, $$D_{\rm ps}\neq0$$. This establishes a **tree-level operator-overlap matching**, not a complete microscopic matching of the $$B=1$$ spectrum.

### 4.3 From Point Splitting to Local Baryon Operators

For the positive transverse-chirality zero mode, the covariant Dirac equation implies, in our conventions,

$$
(D_3-iD_4)v=0
\quad\Longrightarrow\quad
D_4v=-iD_3v.
$$

Consequently,

$$
\boxed{
\epsilon_{abc}v^a(D_3v)^b(D_4v)^c=0.}
$$

This rules out the previously proposed two-derivative color coefficient. Using the local holomorphic representation $$\mathbf u(z)$$ and three nearby points $$z,z+\delta_2,z+\delta_3$$, the Taylor expansion yields

$$
\boxed{
\begin{aligned}
&\det\bigl[\mathbf u(z),\mathbf u(z+\delta_2),
\mathbf u(z+\delta_3)\bigr]\\
&\quad=\frac{\delta_2\delta_3(\delta_3-\delta_2)}{2}
\det[\mathbf u,\mathbf u',\mathbf u'']+O(\delta^4).
\end{aligned}}
$$

Thus, the first **potentially nonzero** local term is $$O(\delta^3)$$ and contains three transverse derivatives. Its color coefficient can be written as

$$
\boxed{
\mathcal W_{210}(y)
=\epsilon_{abc}
(D_3^2v)^a(D_3v)^bv^c.}
$$

An example of a local four-dimensional source with three transverse derivatives is

$$
\boxed{
\mathcal J_h^A(x,y)
=\frac12\epsilon_{abc}\epsilon^{fg}
\bigl[(D_3^2q_f^a)^TC_4\gamma_3(D_3q_g^b)\bigr]
q_h^{cA},}
$$

Its tree-level projection onto three zero modes is proportional to $$\mathcal W_{210}(y)(\xi_R\mathcal B_R+\xi_L\mathcal B_L)$$. In the chosen background, $$\mathcal W_{210}$$ is not identically zero (see the numerical check in Appendix A).

**Note:** A point-split source at finite separation and a derivative-free local Ioffe current are different operators. Nonvanishing overlap of the former does not imply nonvanishing tree-level zero-mode overlap of the latter.

<a id="section-5"></a>

## 5. Non-Abelian Bosonization and Local Factorization [Literature + Derived]

### 5.1 From Two Two-Dimensional Dirac Fields to the $$U(2)_1$$ WZW Model

In the massless leading-order two-dimensional zero-mode theory, two Dirac flavors can be non-Abelian-bosonized into the level-one $$U(2)$$ Wess–Zumino–Witten theory. Define

$$
\boxed{U=e^{i\eta'/2}g,\qquad g\in SU(2),\qquad
\det U=e^{i\eta'}.}
$$

The field $$\eta'$$ is a flavor singlet, whereas $$g$$ transforms as $$g\mapsto LgR^\dagger$$ under $$SU(2)_L\times SU(2)_R$$.

### 5.2 Decomposition of the Kinetic Term

Using

$$
\partial_\mu U=e^{i\eta'/2}
\left[\frac{i}{2}(\partial_\mu\eta')g+\partial_\mu g\right],
$$

together with $$\mathrm{tr}(g^\dagger\partial_\mu g)=\partial_\mu\ln\det g=0$$, we obtain

$$
\boxed{
\mathrm{tr}(\partial_\mu U^\dagger\partial_\mu U)
=\frac12(\partial_\mu\eta')^2
+\mathrm{tr}(\partial_\mu g^\dagger\partial_\mu g).}
$$

With the WZW kinetic normalization $$1/(8\pi)$$, the resulting singlet kinetic term is $$(\partial\eta')^2/(16\pi)$$.

### 5.3 The WZW Three-Form and the Center-Vortex Potential

Write $$A=g^{-1}dg$$. Since

$$
U^{-1}dU=\frac i2d\eta'\,\mathbf{1}+A,
\qquad \mathrm{tr}(A\wedge A)=0,
$$

the local three-form satisfies

$$
\mathrm{tr}(U^{-1}dU)^3
=\mathrm{tr}(g^{-1}dg)^3.
$$

The center-vortex potential depends on $$(\det U)^{\pm1/3}$$ with the appropriate extended-phase definition and therefore only on $$\eta'$$. For massless quarks, the leading-order local action becomes

$$
\boxed{
\begin{aligned}
S_0&=S_{\rm SG}[\eta']+S_{SU(2)_1}[g],\\
S_{\rm SG}[\eta']
&=\int d^2x\left[
\frac{(\partial\eta')^2}{16\pi}
-2\zeta\cos\frac{\eta'-\theta}{3}
\right].
\end{aligned}}
$$

This local action follows from the non-Abelian bosonization and vortex-induced deformation in [2]. **An additive local action does not imply that the physical Hilbert space is a global tensor product**; the $$\mathbb Z_3$$ gluing discussed below must be implemented separately.

### 5.4 Infrared Behavior of the Two Sectors

The canonically normalized field $$\phi=\eta'/\sqrt{8\pi}$$ gives the sine-Gordon coupling $$\beta_{\rm SG}=\sqrt{8\pi}/3$$. The Gaussian scaling dimension of the cosine is

$$
\boxed{\Delta_{\rm vortex}
=\frac{\beta_{\rm SG}^2}{4\pi}=\frac29<2.}
$$

The vortex deformation is therefore relevant and generates a mass scale in the singlet sector; with the full chiral symmetry preserved, the $$SU(2)_1$$ flavor sector remains a massless CFT at leading order. **Quantum corrections and the effects of a particular baryon defect require separate analysis.**

<a id="section-6"></a>

## 6. Topological Baryon Charge and Center Twist [Literature + Conditional]

### 6.1 $$B=1$$ Corresponds to a $$6\pi$$ Winding of $$\eta'$$

The residual $$\mathbb Z_3$$ gauge structure extends the period of the singlet phase:

$$
\eta'\sim\eta'+6\pi.
$$

With the baryon-current normalization corresponding to [2],

$$
\boxed{j_B^\mu
=\frac{1}{6\pi}\epsilon^{\mu\nu}\partial_\nu\eta',
\qquad B=\frac{\Delta\eta'}{6\pi}.}
$$

A candidate $$B=1$$ kink thus has $$\Delta\eta'=6\pi$$.

### 6.2 Global Identification and the Minimal Center-Twist Candidate

For $$N_c=3,N_f=2$$, the covering-space description of the field space includes

$$
\boxed{(\eta',g)\sim(\eta'+6\pi,-g).}
$$

Since $$e^{i(\eta'+6\pi)/2}(-g)=e^{i\eta'/2}g$$, this gluing is compatible with $$U=e^{i\eta'/2}g$$. Along a unit-$$B$$ winding, the most natural flavor candidate is the center twist $$g\mapsto-g$$.

However, **global gluing restricts the allowed topological structure; it does not prove the uniqueness of the microscopic soliton defect dynamics**.

### 6.3 The $$SU(2)_1$$ Twisted Partition Function

The $$SU(2)_1$$ theory has just two integrable representations, $$j=0,\frac12$$, with

$$
h_0=0,\qquad h_{1/2}=\frac14,\qquad c=1.
$$

The partition function with an insertion of the center element is

$$
Z_{\rm ins}=|\chi_0|^2-|\chi_{1/2}|^2.
$$

Using the modular $$S$$ matrix

$$
S=\frac1{\sqrt2}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
$$

one obtains the spatially twisted partition function of the **standard center-twisted model**:

$$
\boxed{Z_{\rm tw}
=\chi_0\bar\chi_{1/2}
+\chi_{1/2}\bar\chi_0.}
$$

The lowest states therefore have

$$
\boxed{(h,\bar h)
=(0,\tfrac14)\ \text{or}\ (\tfrac14,0),
\qquad \Delta_{\min}=\tfrac14.}
$$

The two channels are flavor doublets, giving four components in total at the lowest level. **This is a representation-theoretic result within the specified twisted CFT, not an independent measurement of the lowest four-dimensional QCD spectrum.**

<a id="section-7"></a>

## 7. One-Soliton Threshold Spectral Density [Derived Within the Model]

### 7.1 Singlet–Flavor Factorization of the Baryon Operator

In the minimal factorized description, the lowest-dimension two-dimensional baryon operators can be expressed as

$$
\boxed{
\mathcal B_R\sim\mathcal N_R\mathcal V_{B,R}\Phi_{1/2,L},
\qquad
\mathcal B_L\sim\mathcal N_L\mathcal V_{B,L}\Phi_{1/2,R}.}
$$

The operator $$\mathcal V_B$$ creates the singlet soliton with one unit of baryon number, whereas $$\Phi$$ is a chiral flavor primary with nonzero conformal weight $$h=1/4$$. This product must be interpreted in an allowed global topological sector.

### 7.2 Soft Flavor Spectrum and Threshold Exponent

The two-point function of a chiral CFT primary satisfies

$$
\langle\Phi_h(z)\Phi_h^\dagger(0)\rangle
=\frac{C_f}{z^{2h}}.
$$

Using the Laplace representation

$$
\boxed{
\frac1{z^{2h}}
=\frac1{\Gamma(2h)}
\int_0^\infty d\varepsilon\,
\varepsilon^{2h-1}e^{-\varepsilon z},}
$$

we read off a soft-energy weight $$\propto\varepsilon^{2h-1}$$ for the massless flavor excitations. Assuming a massive soliton of mass $$M_B$$ with a smooth, nonvanishing lowest form factor, one has $$s-M_B^2\propto\varepsilon$$ near threshold. Thus, for the **scalar spectral density after factoring out the light-cone kinematic prefactors**:

$$
\boxed{
\rho_B^{(1)}(s)
\ \propto\ \Theta(s-M_B^2)
(s-M_B^2)^{2h-1}.}
$$

Substituting $$h=1/4$$ gives

$$
\boxed{\alpha=2h-1=-\frac12.}
$$

A more detailed phase-space Jacobian and the form-factor factors are given in Appendix E. This exponent calculation **does not** establish that the chosen one-soliton channel is the lowest physical state, nor does it exclude additional defect scattering phase shifts.

### 7.3 Long-Distance Euclidean Check

For $$x=0$$ and $$M_B\tau\gg1$$, the propagation factor of a massive particle behaves as $$e^{-M_B\tau}/\sqrt\tau$$. Multiplying by the $$SU(2)_1$$ flavor factor $$\tau^{-1/2}$$ yields

$$
\boxed{G_B^{(1)}(\tau,0)
\sim A_G\frac{e^{-M_B\tau}}{\tau}.}
$$

The left- and right-handed candidate operators transform in different $$SU(2)_L\times SU(2)_R$$ representations. If the full chiral symmetry of the massless theory is unbroken, an $$SU(2)_L$$ center transformation implies

$$
\boxed{
G_{RL}=\langle\mathcal B_R\mathcal B_L^\dagger\rangle
=0
\quad\text{(with exact chiral symmetry)}.}
$$

When parity is unbroken and the normalizations are chosen consistently, the two diagonal one-soliton spectral densities have the same threshold form.

<a id="section-8"></a>

## 8. RG Stability, Uniqueness, and Microscopic Obstructions

### 8.1 Bulk and Defect RG Must Be Distinguished

The linear RG eigenvalue of a two-dimensional bulk perturbation is $$2-\Delta$$, while that of a perturbation localized on a one-dimensional defect worldline is

$$
\boxed{\frac{d\widehat\lambda}{d\ell}
=(1-\Delta_{\rm def})\widehat\lambda+\cdots.}
$$

With massless quarks and exact $$SU(2)_L\times SU(2)_R$$ symmetry, $$\\mathrm{tr}g$$ is forbidden, and $$J_L^aJ_R^a$$ is not invariant under the full chiral group. Conventional chirally invariant flavor scalar corrections, such as $$T_f\bar T_f$$, are irrelevant near the fixed point.

On the **standard invertible center line with no additional quantum core**, an allowed stress-tensor coupling takes the form

$$
\delta S_T=\lambda_T\int d\tau\,T_f(\tau,X)
$$

This operator has $$\Delta_T=2$$ and therefore

$$
\boxed{\frac{d\widehat\lambda_T}{d\ell}
=-\widehat\lambda_T+\cdots.}
$$

This supports the **local stability of the specified minimal defect fixed point**, but it is not a complete classification of every microscopic defect operator.

### 8.2 An Illustrative Controlled Bulk-to-Defect Matching

Suppose integrating out high-energy modes induces

$$
\delta S_{\rm mix}
=\frac{c_T}{\Lambda_\perp^2}
\int d^2x\,(\partial\eta')^2 T_f^{xx},
\qquad \Lambda_\perp\sim1/L.
$$

Substituting the classical kink $$\eta'_K$$ and assuming the flavor fields vary slowly over the core scale gives

$$
\int dx\,(\partial_x\eta'_K)^2=72m
\quad\Longrightarrow\quad
\lambda_T\simeq\frac{72c_Tm}{\Lambda_\perp^2}.
$$

Hence, for $$m\ll\Lambda_\perp$$, the dimensionless coupling $$m\lambda_T\sim c_T(m/\Lambda_\perp)^2$$ is suppressed. **Here $$c_T$$ is only an illustrative Wilson coefficient; it has not been computed from loop diagrams in the full four-dimensional QCD theory.**

### 8.3 Exact Flavor-Center Selection Rule

The center of the diagonal $$SU(2)_V$$ acts as $$q\mapsto-q$$. For a color singlet containing $$n_q$$ quarks and $$n_{\bar q}$$ antiquarks,

$$
(-1)^{n_q+n_{\bar q}}
=(-1)^{n_q-n_{\bar q}}
=(-1)^{3B}=(-1)^B.
$$

The center acts on an isospin-$$I$$ representation with the phase $$(-1)^{2I}$$. Consequently,

$$
\boxed{(-1)^{2I}=(-1)^B.}
$$

Ordinary physical $$B=1$$ hadron states must therefore carry half-integer isospin. This is a microscopic symmetry selection rule, but it does not uniquely determine the lowest core dynamics.

### 8.4 How Far Can One Prove Uniqueness of the Lowest Defect?

**Proven within the model:** Once the standard $$SU(2)_1$$ center-twisted Hilbert space is specified, each lowest chiral doublet occurs with multiplicity one and has lowest weight $$1/4$$.

**Microscopic uniqueness remains unproven:** Symmetry permits additional neutral quantum-mechanical core degrees of freedom, in integer-spin flavor representations that do not change the center selection rule, such as

$$
\mathcal H_{\rm core}=(\mathbf3_L,\mathbf3_R).
$$

If this is an additional degenerate core, the effective model may contain

$$
S_{\rm int}=g_K\int d\tau\,
\bigl(S_L^aJ_L^a+S_R^aJ_R^a\bigr).
$$

This interaction is marginal at tree level on a static defect and may generate a new defect RG flow. The construction is **an effective-theory counterexample consistent with the symmetries examined**, not an identified bound state of the four-dimensional QCD theory. Even a decoupled core need not change the exponent $$-1/2$$; the main lesson is that the currently known symmetries alone do not determine the full defect Hilbert space uniquely.

### 8.5 The Indispensable Four-Dimensional Microscopic Matching

To promote the candidate exponent to an unconditional prediction for the lowest baryon spectrum of the microscopic QCD theory, one must answer:

- Are there $$B=1$$ states or continuum thresholds below the candidate soliton channel?
- Are there additional gapless or nearly zero-energy core degrees of freedom?
- Do scattering phase shifts between the real moving soliton and flavor excitations modify the endpoint scaling?
- Is the **full quantum** form factor of the four-dimensional baryon source nonzero in the proposed lowest channel?
- Do the microscopic defect couplings flow into the minimal fixed point described above?

These questions cannot be answered from local factorization of the vacuum EFT, the center-twisted partition function, or the classical fluctuation spectrum of the pure SG kink alone. Lattice calculations can test the predictions but are not logically the only route; new nonperturbative input or controlled microscopic matching is still needed.

<a id="section-9"></a>

## 9. Scope of the Results and Next Questions

| Research question | Present conclusion | Evidence level |
|---|---|---|
| Two-dimensional light fields in flux-compactified small-$$T^2$$ QCD | One two-dimensional Dirac zero mode per flavor | [Literature] |
| Derivative-free, three-zero-mode $$B=1$$ operators | Two doublet types, $$RRL$$ and $$LLR$$ | [Derived] |
| Four-dimensional point-split baryon source | A nonzero tree-level zero-mode projection can be constructed | [Derived] |
| Local low-energy action | Leading-order $$SG\,+\,SU(2)_1$$ | [Literature + Derived] |
| Topological baryon charge | $$B=\Delta\eta'/(6\pi)$$ | [Literature] |
| Lowest weight in the standard center-twisted sector | $$(0,1/4)$$ or $$(1/4,0)$$ | [Derived] |
| One-soliton threshold in the minimal model | $$\rho^{(1)}\sim(s-M_B^2)^{-1/2}$$ | [Conditional] |
| Stress-tensor perturbation of the minimal defect | Infrared irrelevant | [Derived: restricted operator space] |
| Microscopic uniqueness of the lowest defect | Not implied by the currently known symmetries | [Open] |
| Microscopic core spectrum, scattering phase shifts, and RG initial conditions | Matching not completed | [Open] |

**Most precise statement of the research at present:**

> Starting from small-$$T^2$$ QCD with baryon-'t Hooft flux, one can construct candidate two-dimensional baryon operators with a definite microscopic zero-mode origin and exhibit four-dimensional sources whose tree-level projections onto them are nonzero. Within the leading $$SG\times SU(2)_1$$ description, the lowest flavor weight of the standard center-twisted sector is $$1/4$$. If the physical infrared $$B=1$$ defect is governed by this minimal channel, with no lower-lying states or additional core scattering that modifies the threshold, the one-soliton spectral density has exponent $$-1/2$$. Neither the microscopic defect fixed point nor the full lowest spectrum has yet been independently established.

---

<a id="appendix-a"></a>

## Appendix A: Explicit Transverse Zero-Mode Wavefunctions and a Nonzero Wronskian

In the local gauge used in [1], define

$$
X=\frac{x_3}{L},\quad Y=\frac{x_4}{L},\quad
z=X-iY,
$$

A zero-mode solution compatible with the chosen gauge convention is

$$
\boxed{v^a(y)=\mathcal N_\perp e^{-\pi X^2/3}u_a(z),\qquad
u_a(z)=\sum_{n\in\mathbb Z}
\exp\!\left[-3\pi\left(n+\frac{a-1}{3}\right)^2
+2\pi\left(n+\frac{a-1}{3}\right)z\right].}
$$

The corresponding twisted boundary conditions are implemented by clock and shift matrices. The components $$u_a$$ are local sections, not ordinary globally periodic scalar functions on the torus.

A determinant formed from the holomorphic color vectors evaluated at three transversely separated points can be checked directly:

$$
\det[\mathbf u(0),\mathbf u(1/3),\mathbf u(2/3)]
\simeq 0.12553202345\ne0,
$$

and

$$
\det[\mathbf u(0),\mathbf u'(0),\mathbf u''(0)]
\simeq2.42169200583\ne0.
$$

These values are obtained by direct summation of the **dimensionless series in the chosen gauge**; they are not four-dimensional lattice-QCD spectral data. After accounting for the corresponding common Gaussian factors and Wilson lines, they establish the existence of nonzero tree-level zero-mode color coefficients.

A short verification script (Python 3 + NumPy):

```python
import numpy as np

n = np.arange(-25, 26)

def u(z, derivative=0):
    values = []
    for a in range(3):
        t = n + a / 3.0
        values.append(np.sum(
            np.exp(-3 * np.pi * t**2 + 2 * np.pi * t * z)
            * (2 * np.pi * t)**derivative
        ))
    return np.asarray(values)

D_split = np.linalg.det(np.column_stack([u(0), u(1/3), u(2/3)]))
D_W     = np.linalg.det(np.column_stack([u(0), u(0, 1), u(0, 2)]))
print('split determinant =', D_split)
print('Wronskian         =', D_W)
```

The local three-derivative baryon source still carries the background flux associated with total $$B=1$$. Its transverse coefficient must therefore be treated as a charged section. To obtain a source depending only on two-dimensional coordinates, one may smear it against a test section $$w_B(y)$$ with the same transformation law, using $$\int_{T^2}d^2y\,w_B^*(y)\mathcal J_{4d}(x,y)$$.

<a id="appendix-b"></a>

## Appendix B: Step-by-Step Decomposition $$U(2)_1\to SG+SU(2)_1$$

Write $$U=e^{i\eta'/2}g$$. Then

$$
\begin{aligned}
\partial_\mu U&=e^{i\eta'/2}
\left(\partial_\mu g+\frac i2(\partial_\mu\eta')g\right),\\
\partial_\mu U^\dagger&=
\left(\partial_\mu g^\dagger-\frac i2(\partial_\mu\eta')g^\dagger\right)e^{-i\eta'/2}.
\end{aligned}
$$

Expanding the four terms, the traces of the mixed terms are proportional to $$\\mathrm{tr}(g^\dagger\partial_\mu g)=0$$, while $$\\mathrm{tr}(g^\dagger g)=2$$. Thus

$$
\\mathrm{tr}(\partial U^\dagger\partial U)
=\\mathrm{tr}(\partial g^\dagger\partial g)+\frac12(\partial\eta')^2.
$$

With $$A=g^{-1}dg$$ and $$a=(i/2)d\eta'$$, we have $$U^{-1}dU=A+a\\mathbf{1}$$ and $$a\wedge a=0$$:

$$
\\mathrm{tr}(A+a\\mathbf{1})^3
=\\mathrm{tr}A^3+3a\wedge\\mathrm{tr}(A\wedge A)
=\\mathrm{tr}A^3.
$$

Finally, because $$\det U=e^{i\eta'}$$, the vortex vertex in the original paper,

$$
-e^{i\theta/3}(\det U)^{-1/3}+\text{h.c.}
$$

becomes $$-2\cos[(\eta'-\theta)/3]$$ after absorbing the appropriate coefficient into $$\zeta$$. The global $$\mathbb Z_3$$ identification is not removed by this local algebraic decomposition.

<a id="appendix-c"></a>

## Appendix C: Classical Sine-Gordon Kink and Fluctuation Spectrum

Use the static energy functional with the vacuum energy subtracted:

$$
E[\eta']=\int dx\left[
\frac{(\partial_x\eta')^2}{16\pi}
+2\zeta\left(1-\cos\frac{\eta'}3\right)\right].
$$

With $$m^2=16\pi\zeta/9$$, the classical solution satisfying $$\Delta\eta'=6\pi$$ is

$$
\boxed{\eta'_K(x)=12\arctan e^{m(x-X)},\qquad
\partial_x\eta'_K(x)=6m\,\\mathrm{sech}[m(x-X)].}
$$

Direct integration gives

$$
\int dx\,(\partial_x\eta'_K)^2
=36m^2\int dx\,\\mathrm{sech}^2[m(x-X)]
=72m.
$$

The first-integral relation gives the classical kink mass:

$$
\boxed{M_K^{\rm cl}=\frac{1}{8\pi}\,72m=\frac{9m}{\pi}.}
$$

This is not the exact soliton mass in the quantum sine-Gordon theory. The linearized fluctuations obey

$$
\boxed{H_K=-\partial_x^2+m^2\left[1-2\\mathrm{sech}^2(m(x-X))\right]
=A^\dagger A,\qquad
A=\partial_x+m\tanh(m(x-X)).}
$$

The normalizable zero mode $$\psi_0\propto\\mathrm{sech}(m(x-X))$$ corresponds to center-of-mass translation. There is no other normalizable discrete shape-bound state, and the continuum starts at $$\omega^2=m^2$$. **This only constrains classical singlet fluctuations in the pure SG model; it does not exclude additional composite core states in four-dimensional QCD.**

<a id="appendix-d"></a>

## Appendix D: Finite-Volume Spectrum of the Standard Center Twist

If the remaining spatial direction is also compactified with circumference $$R$$, the flavor CFT energy is

$$
E_f(R)=\frac{2\pi v}{R}
\left(h+\bar h-\frac{c}{12}\right),
\qquad c=1.
$$

The lowest twisted level has $$h+\bar h=1/4$$, so its energy difference from the untwisted vacuum is

$$
\boxed{\Delta E_f(R)=\frac{2\pi v}{R}\cdot\frac14
=\frac{\pi v}{2R}.}
$$

Assuming **minimal factorization, suitable topological boundary conditions, and no additional $$1/R$$ contribution from defect scattering phase shifts**, one may consider the fit

$$
E_{B=1}(R)-E_{B=0}(R)
=M_B+\frac{\pi v}{2R}+\cdots.
$$

The low-order expansions of the corresponding $$SU(2)_1$$ characters are

$$
\begin{aligned}
\chi_0(q)&=q^{-1/24}(1+3q+4q^2+7q^3+13q^4+\cdots),\\
\chi_{1/2}(q)&=q^{5/24}(2+2q+6q^2+8q^3+14q^4+\cdots).
\end{aligned}
$$

Combining the two chiral channels and setting $$q=\bar q$$ for a formal energy-level count gives the degeneracy sequence

$$
\boxed{d_n=4,\ 16,\ 40,\ 96,\ 204,\ldots}
$$

This applies only to the standard twisted CFT. It excludes the translational momentum tower of the mobile soliton and any possible core Hilbert space, and it is not four-dimensional lattice-QCD data.

<a id="appendix-e"></a>

## Appendix E: Phase-Space Derivation and Normalization of the One-Soliton Spectral Density

For a chiral soft mode, use

$$
\frac1{z^{1/2}}=\frac1{\sqrt\pi}
\int_0^\infty d\varepsilon\,
\varepsilon^{-1/2}e^{-\varepsilon z}.
$$

Let the soliton rapidity be $$\vartheta$$, with momentum

$$
p_{\rm sol}^0=M\cosh\vartheta,
\qquad p_{\rm sol}^1=M\sinh\vartheta.
$$

Combining it with a right-moving soft mode $$p_f=(\varepsilon,\varepsilon)$$ gives

$$
\begin{aligned}
P^0&=M\cosh\vartheta+\varepsilon,\\
P^1&=M\sinh\vartheta+\varepsilon,\\
s=P^2&=M^2+2M\varepsilon e^{-\vartheta}.
\end{aligned}
$$

The Jacobian for the change of variables is

$$
\left|\frac{\partial(P^0,P^1)}
{\partial(\vartheta,\varepsilon)}\right|
=M e^{-\vartheta}=P_-.
$$

For the appropriate topological vertex, the one-soliton form factor has rapidity dependence $$\lvert F_L(\vartheta)\rvert^2\propto e^{-3\vartheta/2}$$ in our left/right convention and the normalization framework of [3] (the right-handed expression is related by parity). The phase-space integral then contains

$$
\frac{|F_L(\vartheta)|^2\,\varepsilon^{-1/2}}{P_-}
\ \propto\ P_-\,(s-M^2)^{-1/2}.
$$

Thus, after extracting the fixed $$P_-$$ kinematic prefactor,

$$
\boxed{\rho_L^{(1)}(s)=A_L
\frac{\Theta(s-M^2)}{\sqrt{s-M^2}}.}
$$

The coefficient $$A_L$$ includes normalization of the two-dimensional operator, the singlet-soliton form factor, and the four-dimensional source-matching coefficient; it cannot be determined from the $$SU(2)_1$$ conformal weight alone. Parity and matching normalizations give the corresponding $$\rho_R^{(1)}$$. The convention used to factor out $$P_\pm$$ must be kept consistent across different tensor decompositions of the spectral density.

<a id="references"></a>

## References

1. Y. Tanizaki and M. Ünsal, *Center vortex and confinement in Yang–Mills theory and QCD with anomaly-preserving compactifications*, **PTEP 2022**, 04A108, [arXiv:2201.06166](https://arxiv.org/abs/2201.06166), [DOI](https://doi.org/10.1093/ptep/ptac042). — The original flux-compactification background and zero-mode analysis.
2. Y. Hayashi and Y. Tanizaki, *Semiclassics for the QCD vacuum structure through $$T^2$$-compactification with the baryon-'t Hooft flux*, **JHEP 08 (2024) 001**, [arXiv:2402.04320](https://arxiv.org/abs/2402.04320), [DOI](https://doi.org/10.1007/JHEP08(2024)001). — The residual $$\mathbb Z_3$$, non-Abelian bosonization, extended periodicity of $$\eta'$$, and the vacuum effective action.
3. S. Lukyanov and A. B. Zamolodchikov, *Form factors of soliton-creating operators in the sine-Gordon model*, **Nucl. Phys. B 607 (2001) 437–455**, [arXiv:hep-th/0102079](https://arxiv.org/abs/hep-th/0102079), [DOI](https://doi.org/10.1016/S0550-3213(01)00262-0). — The form-factor approach for soliton-creating vertices.

---

*Note: This article distinguishes structures established directly in the cited literature from subsequent derivations within a specified model. The outstanding microscopic matching of the four-dimensional low-energy spectrum must not be omitted when citing these results.*
