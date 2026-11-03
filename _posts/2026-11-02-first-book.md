---
title: "Small-$T^2$ QCD 中的重子算符、拓扑孤子与连续谱阈值：研究进展与证明边界"
date: 2026-11-02
permalink: /posts/2026/11/qcd-t2-baryon-threshold/
excerpt: "从四维带重子磁通 QCD 的横向零模出发，研究最低维重子算符、非阿贝尔玻色化、中心扭曲以及重子谱密度的阈值行为，并区分已证明结果与开放问题。"
tags:
  - QCD
  - compactification
  - baryon
  - WZW
  - sine-Gordon
  - spectral-density
math: true
---

> **研究笔记（2026-11-03 修订）**  本文整理一个正在推进的解析研究计划，而不是宣称已经证明原始四维 QCD 的最低重子谱。文中用 **[文献]**、**[推导]**、**[条件]**、**[待证]** 标记不同证据层次。涉及算符的公式均采用本文的归一化、手征和背景规范约定。

## 摘要

考虑两个无质量 flavor 的 $SU(3)$ QCD，在

$$
\mathbb R^{1,1}\times T^2,
\qquad N_c=3,\quad N_f=2,\quad L\Lambda_{\rm QCD}\ll1
$$

上施加兼容的颜色 't Hooft flux 与重子数磁通。原有研究建立了从四维背景到二维 Dirac 零模以及 center-vortex 有效理论的联系。本文进一步整理以下研究：

1. 将二维无导数的最低维 $B=1$ 算符完整分类为两类手征 doublet；
2. 构造具有非零树级零模投影的四维 point-split 重子源，并厘清其局域导数展开；
3. 将 $U(2)_1$ WZW 的领先阶局部作用量分解成 sine-Gordon singlet sector 与 $SU(2)_1$ flavor sector；
4. 将 $B=1$ 与 $\eta'$ 的 $6\pi$ winding 对应，计算**标准中心扭曲模型**的最低 conformal weight；
5. 在单 soliton form factor 非零、因子化且无危险缺陷相互作用的假设下，得到谱密度阈值指数 $\alpha=-1/2$；
6. 讨论缺陷 RG、核心自由度的对称性允许反例，以及尚未完成的四维微观匹配。

**中心结论（条件性）：**

$$
\boxed{\rho_B^{(1)}(s)\ \sim\ A_B\,
\Theta(s-M_B^2)(s-M_B^2)^{-1/2}}
$$

是**最小因子化缺陷模型中的最低单 soliton 连续谱贡献**，尚不是完整四维 QCD 的无条件最低谱定理。

---

## 目录

1. [研究目标与逻辑链](#section-1)
2. [四维磁通紧致化与二维零模](#section-2)
3. [最低维二维重子算符的分类](#section-3)
4. [四维重子源与 point-splitting 匹配](#section-4)
5. [非阿贝尔玻色化及局部因子化](#section-5)
6. [重子数拓扑荷与中心扭曲](#section-6)
7. [单 soliton 阈值谱密度](#section-7)
8. [RG 稳定性、唯一性与微观障碍](#section-8)
9. [结果边界与下一步问题](#section-9)
10. [附录 A：横向波函数及 Wronskian](#appendix-a)
11. [附录 B：WZW 动能与三形式的分解](#appendix-b)
12. [附录 C：经典 kink 及涨落谱](#appendix-c)
13. [附录 D：中心扭曲有限体积谱](#appendix-d)
14. [附录 E：谱密度的相空间推导](#appendix-e)
15. [参考文献](#references)

<a id="section-1"></a>
## 1. 研究目标与逻辑链

我们尝试建立的逻辑链是

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

**必须强调：** 从 $B=1$ 的全局约束到“无附加核心自由度的最小缺陷固定点”是目前最重要的**待证动力学箭头**。二维模型的自洽计算不能替代这个匹配。

记号约定：$L$ 表示横向 $T^2$ 尺度；$R$ 表示进一步有限化后纵向空间圆周的长度；$M_B$ 表示最低候选 soliton 的物理质量，不等同于经典小涨落质量。

<a id="section-2"></a>
## 2. 四维磁通紧致化与二维零模 [文献]

将四维坐标记为 $X=(x,y)$，其中 $x\in\mathbb R^{1,1}$，$y=(x_3,x_4)\in T^2$。在单位重子磁通背景中，

$$
\int_{T^2}F_B=2\pi.
$$

颜色 twist 与重子磁通结合，使夸克的横向 Dirac 算符具有一个规范允许的零模（每个 flavor 对应一个二维 Dirac 场），而非零横向激发的典型能标为 $O(1/L)$ [1,2]。

四维夸克场可展开为

$$
\boxed{
q_f^{aA}(x,y)
=v^a(y)\bigl[\xi_R^A\chi_{f,R}(x)
+\xi_L^A\chi_{f,L}(x)\bigr]
+q_{f,H}^{aA}(x,y).}
$$

这里 $a=1,2,3$ 是颜色指标，$A$ 是四维 Dirac 指标；$v^a(y)$ 是横向颜色波函数，$\xi_{R,L}$ 为固定的自旋嵌入，$\chi_{f,R/L}(x)$ 为**无独立颜色指标**的二维 Grassmann 场。适当归一化为

$$
\int_{T^2}d^2y\sum_{a=1}^3|v^a(y)|^2=1.
$$

因此，最低能量的 flavor 场空间是

$$
U_R=\operatorname{span}\{\chi_{u,R},\chi_{d,R}\}
\simeq\mathbf2_R,
\qquad
U_L\simeq\mathbf2_L.
$$

**结论：** 原始紧致化背景支持二维低能场的构造；但“非零 KK 模在真空背景中有隙”并不等于“相互作用重子核心不存在新低能态”。

<a id="section-3"></a>
## 3. 最低维二维重子算符的分类 [推导]

### 3.1 由 Grassmann 反对易关系分类

研究不含导数、由三个二维零模费米场构成、经典维数 $\Delta_{\rm UV}=3/2$ 的 $B=1$ 算符。三个 Grassmann 生成元的反对称组合属于

$$
\Lambda^3(U_R\oplus U_L)
=\Lambda^3U_R
\oplus(\Lambda^2U_R\otimes U_L)
\oplus(U_R\otimes\Lambda^2U_L)
\oplus\Lambda^3U_L.
$$

因为 $\dim U_R=\dim U_L=2$，有

$$
\Lambda^3U_R=\Lambda^3U_L=0,
\qquad \Lambda^2\mathbf2=\mathbf1.
$$

从而

$$
\boxed{
\Lambda^3(\mathbf2_R\oplus\mathbf2_L)
=(\mathbf1_R,\mathbf2_L)\oplus(\mathbf2_R,\mathbf1_L).}
$$

所以 $RRR$ 与 $LLL$ 组合消失，最低维算符仅有 $RRL$ 和 $LLR$ 两类。取 $\epsilon^{ud}=1$，定义

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

例如 $\mathcal B_R^u=:\!\chi_{u,R}\chi_{d,R}\chi_{u,L}\!:$。两类算符在对角 $SU(2)_V$ 下都是 $I=1/2$ doublet，不包含额外的 $I=3/2$ 分量。

### 3.2 Lorentz 标签与 flavor 表示不可混淆

二维基本费米场的 Lorentz 权重取 $s(\chi_R)=+1/2$、$s(\chi_L)=-1/2$。于是

$$
\begin{aligned}
s(\mathcal B_R)&=+\frac12+\frac12-\frac12=+\frac12,\\
s(\mathcal B_L)&=-\frac12-\frac12+\frac12=-\frac12.
\end{aligned}
$$

这解释了为什么复合算符的下标分别为 $R$ 与 $L$；另一方面，$SU(2)_R$ singlet 来自两只右手场的 flavor 反对称收缩，所以

$$
\mathcal B_R\sim(\mathbf1_R,\mathbf2_L),\qquad
\mathcal B_L\sim(\mathbf2_R,\mathbf1_L).
$$

**适用范围：** 这里证明的“恰有两类”只限于**二维、纯零模、无导数、最低经典维数**的算符空间，不能推广为“四维所有重子源只有两类”。

<a id="section-4"></a>
## 4. 四维重子源与 point-splitting 匹配 [推导]

### 4.1 普通局域三夸克源的树级投影为何为零？

考虑一般的局域四维重子源（Dirac 张量省略）：

$$
\mathcal J_{\rm loc}(x,y)
=\epsilon_{abc}\,q^a(x,y)q^b(x,y)q^c(x,y).
$$

所有夸克都取相同横向零模时，颜色系数为

$$
\boxed{
\epsilon_{abc}v^a(y)v^b(y)v^c(y)
=\det[v(y),v(y),v(y)]=0.}
$$

所以**无横向导数的局域三夸克源**的树级纯零模投影为零；这不意味着它的全阶量子匹配系数为零，更不意味着二维 $\mathcal B_{R,L}$ 算符不存在。

### 4.2 带 Wilson line 的 point-split 源

在横向 $T^2$ 取三个位置 $y_i$ 与公共基点 $y_0$，定义

$$
\widehat q_f(x;y_i,y_0)
=W(y_0,y_i)q_f(x,y_i),
$$

其中 $W$ 为沿指定路径的背景及颜色平行输运。定义四维 Dirac 旋量值源

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

在颜色规范变换下它不变；作为总 $B=1$ 的算符，它在外加 $U(1)_B$ 背景变换下仍是带电、规范**协变**的源。将零模展开代入，得到

$$
\boxed{
P_0\mathcal J_{h,\rm ps}^{A}
=D_{\rm ps}(y_1,y_2,y_3;y_0)
\bigl[\xi_R^A\mathcal B_R^h
+\xi_L^A\mathcal B_L^h\bigr],}
$$

其中整体相位取决于 Dirac 基和路径约定，且

$$
D_{\rm ps}
=\epsilon_{abc}
\widehat v^a(y_1)\widehat v^b(y_2)\widehat v^c(y_3).
$$

因此，只要三个平行输运后的颜色向量线性独立，就有 $D_{\rm ps}\ne0$。这是**树级算符存在性匹配**，不是完整 $B=1$ 微观能谱匹配。

### 4.3 重要修正：最早的 $O(\delta^2)$ 展开是错误的

对于当前横向正手性零模，协变 Dirac 方程给出（在本文约定下）

$$
(D_3-iD_4)v=0
\quad\Longrightarrow\quad
D_4v=-iD_3v.
$$

因此

$$
\boxed{
\epsilon_{abc}v^a(D_3v)^b(D_4v)^c=0.}
$$

这排除了以前设想的二导数颜色系数。取局部全纯表示 $\mathbf u(z)$ 和相近的三个点 $z,z+\delta_2,z+\delta_3$，Taylor 展开得

$$
\boxed{
\begin{aligned}
&\det\bigl[\mathbf u(z),\mathbf u(z+\delta_2),
\mathbf u(z+\delta_3)\bigr]\\
&\quad=\frac{\delta_2\delta_3(\delta_3-\delta_2)}{2}
\det[\mathbf u,\mathbf u',\mathbf u'']+O(\delta^4).
\end{aligned}}
$$

所以首个**可能非零**的局域项是 $O(\delta^3)$，对应三个横向导数。它的颜色系数可写作

$$
\boxed{
\mathcal W_{210}(y)
=\epsilon_{abc}
(D_3^2v)^a(D_3v)^bv^c.}
$$

例如，含三导数的局域四维源为

$$
\boxed{
\mathcal J_h^A(x,y)
=\frac12\epsilon_{abc}\epsilon^{fg}
\bigl[(D_3^2q_f^a)^TC_4\gamma_3(D_3q_g^b)\bigr]
q_h^{cA},}
$$

它的树级纯零模投影与 $\mathcal W_{210}(y)(\xi_R\mathcal B_R+\xi_L\mathcal B_L)$ 成正比。在所选背景下，$\mathcal W_{210}$ 不恒为零（数值检查见附录 A）。

**注意：** 有限分离的 point-split 源与无导数的局域 Ioffe current 是不同的算符；前者非零不证明后者具有非零树级零模重叠。

<a id="section-5"></a>
## 5. 非阿贝尔玻色化及局部因子化 [文献 + 推导]

### 5.1 从两个二维 Dirac 场到 $U(2)_1$ WZW

在无质量、领先阶二维零模理论中，两个 Dirac flavor 可以非阿贝尔玻色化成 level-1 的 $U(2)$ Wess–Zumino–Witten 理论。定义

$$
\boxed{U=e^{i\eta'/2}g,\qquad g\in SU(2),\qquad
\det U=e^{i\eta'}.}
$$

$\eta'$ 为 singlet 场，$g$ 在 $SU(2)_L\times SU(2)_R$ 下按 $g\mapsto LgR^\dagger$ 变换。

### 5.2 动能项分解

由

$$
\partial_\mu U=e^{i\eta'/2}
\left[\frac{i}{2}(\partial_\mu\eta')g+\partial_\mu g\right],
$$

以及 $\operatorname{tr}(g^\dagger\partial_\mu g)
=\partial_\mu\ln\det g=0$，得到

$$
\boxed{
\operatorname{tr}(\partial_\mu U^\dagger\partial_\mu U)
=\frac12(\partial_\mu\eta')^2
+\operatorname{tr}(\partial_\mu g^\dagger\partial_\mu g).}
$$

在 $1/(8\pi)$ 的 WZW 动能归一化下，singlet 动能因此是 $(\partial\eta')^2/(16\pi)$。

### 5.3 WZW 三形式与 center-vortex 势

记 $A=g^{-1}dg$。因为

$$
U^{-1}dU=\frac i2d\eta'\,\mathbf1+A,
\qquad \operatorname{tr}(A\wedge A)=0,
$$

所以局部三形式满足

$$
\operatorname{tr}(U^{-1}dU)^3
=\operatorname{tr}(g^{-1}dg)^3.
$$

而 center-vortex 势取决于扩展意义下的 $(\det U)^{\pm1/3}$，因而只依赖 $\eta'$。在无质量条件下，领先阶局部作用量得到

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

以上局部作用量来源于 [2] 的非阿贝尔玻色化和 vortex 变形。**局部相加并不自动意味着物理 Hilbert space 是全局直积**；下面的 $\mathbb Z_3$ gluing 必须另行处理。

### 5.4 两个 sector 的红外行为

规范归一化 $\phi=\eta'/\sqrt{8\pi}$ 给出 sine-Gordon 耦合 $\beta_{\rm SG}=\sqrt{8\pi}/3$。cosine 的 Gaussian 维数为

$$
\boxed{\Delta_{\rm vortex}
=\frac{\beta_{\rm SG}^2}{4\pi}=\frac29<2.}
$$

因此 vortex 形变相关，使 singlet sector 获得质量尺度；保持完整手征对称性时，$SU(2)_1$ flavor sector 在领先阶仍是无质量 CFT。**量子修正和特定重子缺陷对该陈述的影响需要另行分析**。

<a id="section-6"></a>
## 6. 重子数拓扑荷与中心扭曲 [文献 + 条件]

### 6.1 $B=1$ 对应 $\eta'$ 的 $6\pi$ winding

残余 $\mathbb Z_3$ 规范结构使 singlet 相位具有扩展周期

$$
\eta'\sim\eta'+6\pi.
$$

采用 [2] 所对应的重子流规范化，

$$
\boxed{j_B^\mu
=\frac{1}{6\pi}\epsilon^{\mu\nu}\partial_\nu\eta',
\qquad B=\frac{\Delta\eta'}{6\pi}.}
$$

因此 $B=1$ 的候选 kink 满足 $\Delta\eta'=6\pi$。

### 6.2 全局识别与最小中心扭曲候选

对于 $N_c=3,N_f=2$，场空间的覆盖描述包含

$$
\boxed{(\eta',g)\sim(\eta'+6\pi,-g).}
$$

因为 $e^{i(\eta'+6\pi)/2}(-g)=e^{i\eta'/2}g$，该 gluing 与 $U=e^{i\eta'/2}g$ 相容。沿 $B=1$ winding，最自然的 flavor 候选是 $g\mapsto-g$ 的中心扭曲。

但**全局 gluing 只约束允许的拓扑结构，不直接证明微观 soliton 的唯一缺陷动力学**。

### 6.3 $SU(2)_1$ 扭曲配分函数

$SU(2)_1$ 只有 $j=0,\frac12$ 两个可积表示，对应

$$
h_0=0,\qquad h_{1/2}=\frac14,\qquad c=1.
$$

中心插入后的配分函数为

$$
Z_{\rm ins}=|\chi_0|^2-|\chi_{1/2}|^2.
$$

利用 modular $S$ 矩阵

$$
S=\frac1{\sqrt2}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
$$

可得到**标准中心扭曲模型**的空间扭曲配分函数

$$
\boxed{Z_{\rm tw}
=\chi_0\bar\chi_{1/2}
+\chi_{1/2}\bar\chi_0.}
$$

因此最低态具有

$$
\boxed{(h,\bar h)
=(0,\tfrac14)\ \text{或}\ (\tfrac14,0),
\qquad \Delta_{\min}=\tfrac14.}
$$

两个通道分别是 flavor doublet，合计最低层四个分量。**此结论是固定扭曲 CFT 的表示论结果，而不是原始四维 QCD 的独立最低谱测量。**

<a id="section-7"></a>
## 7. 单 soliton 阈值谱密度 [模型内推导]

### 7.1 重子算符的 singlet–flavor 分解

在最小因子化描述中，最低二维重子算符可表示为

$$
\boxed{
\mathcal B_R\sim\mathcal N_R\mathcal V_{B,R}\Phi_{1/2,L},
\qquad
\mathcal B_L\sim\mathcal N_L\mathcal V_{B,L}\Phi_{1/2,R}.}
$$

$\mathcal V_B$ 创造单位重子数的 singlet soliton，$\Phi$ 是手征 flavor primary，其非零权重为 $h=1/4$。此处的乘积分解必须在允许的全局拓扑扇区中理解。

### 7.2 软 flavor 谱与阈值指数

手征 CFT 的两点函数满足

$$
\langle\Phi_h(z)\Phi_h^\dagger(0)\rangle
=\frac{C_f}{z^{2h}}.
$$

使用 Laplace 表示

$$
\boxed{
\frac1{z^{2h}}
=\frac1{\Gamma(2h)}
\int_0^\infty d\varepsilon\,
\varepsilon^{2h-1}e^{-\varepsilon z},}
$$

可读出无质量 flavor 的软能量权重 $\propto\varepsilon^{2h-1}$。在一个有质量 soliton 质量为 $M_B$、其最低 form factor 光滑且非零的假设下，阈值附近 $s-M_B^2\propto\varepsilon$。于是对于**已提取轻锥运动学因子的标量谱密度**，

$$
\boxed{
\rho_B^{(1)}(s)
\ \propto\ \Theta(s-M_B^2)
(s-M_B^2)^{2h-1}.}
$$

代入 $h=1/4$：

$$
\boxed{\alpha=2h-1=-\frac12.}
$$

更完整的相空间 Jacobian 与 form-factor 因子见附录 E。这个指数计算**没有**证明最低物理态必然就是所选单 soliton 通道，也没有排除新的缺陷散射相移。

### 7.3 Euclidean 长距离检验

有质量单粒子传播因子在 $x=0$、$M_B\tau\gg1$ 时近似为 $e^{-M_B\tau}/\sqrt\tau$；乘上 $SU(2)_1$ flavor 因子 $\tau^{-1/2}$，得到

$$
\boxed{G_B^{(1)}(\tau,0)
\sim A_G\frac{e^{-M_B\tau}}{\tau}.}
$$

左右候选算符属于不同的 $SU(2)_L\times SU(2)_R$ 表示。如果无质量理论的完整手征对称性未破缺，则利用 $SU(2)_L$ 中心变换，

$$
\boxed{
G_{RL}=\langle\mathcal B_R\mathcal B_L^\dagger\rangle
=0
\quad\text{（精确手征对称性下）}.}
$$

宇称对称且归一化一致时，两条对角单 soliton 谱具有相同的阈值形式。

<a id="section-8"></a>
## 8. RG 稳定性、唯一性与微观障碍

### 8.1 Bulk RG 与 defect RG 必须分开

对二维 bulk 扰动，线性 RG 本征值为 $2-\Delta$；对一维缺陷世界线上的扰动，则为

$$
\boxed{\frac{d\widehat\lambda}{d\ell}
=(1-\Delta_{\rm def})\widehat\lambda+\cdots.}
$$

在无质量、完整 $SU(2)_L\times SU(2)_R$ 对称下，$\operatorname{tr}g$ 不允许，$J_L^aJ_R^a$ 也不在完整手征群下不变。保持完整手征对称性的普通 flavor 标量修正，如 $T_f\bar T_f$，在固定点附近为无关算符。

对于**没有附加量子核心的标准可逆中心线**，线上的应力张量耦合

$$
\delta S_T=\lambda_T\int d\tau\,T_f(\tau,X)
$$

具有 $\Delta_T=2$，因此

$$
\boxed{\frac{d\widehat\lambda_T}{d\ell}
=-\widehat\lambda_T+\cdots.}
$$

这支持**特定最小缺陷固定点的局部稳定性**，但并非所有微观缺陷算符的完整分类。

### 8.2 受控的示例性 bulk-to-defect 匹配

若高能模诱导

$$
\delta S_{\rm mix}
=\frac{c_T}{\Lambda_\perp^2}
\int d^2x\,(\partial\eta')^2 T_f^{xx},
\qquad \Lambda_\perp\sim1/L,
$$

将经典 kink $\eta'_K$ 代入，并假设 flavor 场在核心尺度上变化缓慢，则

$$
\int dx\,(\partial_x\eta'_K)^2=72m
\quad\Longrightarrow\quad
\lambda_T\simeq\frac{72c_Tm}{\Lambda_\perp^2}.
$$

故 $m\ll\Lambda_\perp$ 时，无量纲 $m\lambda_T\sim c_T(m/\Lambda_\perp)^2$ 受抑制。**这里的 $c_T$ 只是示意性 Wilson coefficient，尚未从完整四维 QCD 的圈图求出。**

### 8.3 精确 flavor 中心选择定则

对角 $SU(2)_V$ 的中心作用为 $q\mapsto-q$。对于含有 $n_q$ 个夸克与 $n_{\bar q}$ 个反夸克的颜色 singlet，

$$
(-1)^{n_q+n_{\bar q}}
=(-1)^{n_q-n_{\bar q}}
=(-1)^{3B}=(-1)^B.
$$

自旋 $I$ 表示中的中心相位为 $(-1)^{2I}$，故

$$
\boxed{(-1)^{2I}=(-1)^B.}
$$

于是 $B=1$ 的通常物理强子态必须具有半整数 isospin。这是一条微观对称性选择定则；但它不能唯一确定最低核心动力学。

### 8.4 “最低缺陷唯一”可以证明到哪一步？

**模型内已证明：** 固定标准 $SU(2)_1$ 中心扭曲 Hilbert space 后，每个最低手征 doublet 只出现一次，其最低权重为 $1/4$。

**微观唯一性未证明：** 对称性允许在最小扭曲缺陷之外增加不改变中心选择定则的中性量子力学核心，例如整数 flavor 表示

$$
\mathcal H_{\rm core}=(\mathbf3_L,\mathbf3_R).
$$

取其为额外简并核心，模型可含

$$
S_{\rm int}=g_K\int d\tau\,
\bigl(S_L^aJ_L^a+S_R^aJ_R^a\bigr).
$$

该耦合在静态缺陷上树级边缘，可能产生新的缺陷 RG 流。这个构造只是**与所检查对称性相容的有效理论反例**，并不是已经在四维 QCD 中发现了此核心束缚态。即使有解耦核心，也未必改变 $-1/2$ 指数；它首先说明仅靠现有对称性不能唯一确定完整缺陷 Hilbert space。

### 8.5 不能省略的四维微观匹配

要将候选指数提升为原始 QCD 最低重子谱的无条件预测，还需回答：

- 是否存在比候选 soliton 更低的 $B=1$ 态或更低的连续谱阈值？
- 是否存在额外无隙或近零能核心自由度？
- 真实的移动 soliton–flavor 散射相移是否改变端点标度？
- 四维重子源的**完整量子** form factor 对目标最低通道是否非零？
- 微观缺陷耦合是否流向上述最小固定点？

这些信息不能由普通真空 EFT 的局部因子化、中心扭曲配分函数或纯 SG kink 的经典涨落谱单独确定。格点可作为检验方法，但并非逻辑上唯一的途径；仍需新的非微扰或受控匹配计算。

<a id="section-9"></a>
## 9. 结果边界与下一步问题

| 研究问题 | 目前结论 | 证据层级 |
|---|---|---|
| 带磁通 small-$T^2$ 的二维轻自由度 | 每 flavor 一个二维 Dirac 零模 | [文献] |
| 无导数三零模 $B=1$ 算符分类 | $RRL$ 与 $LLR$ 两类 doublet | [推导] |
| 四维 point-split 重子源 | 可构造非零树级零模投影 | [推导] |
| 局域低能作用量 | 领先阶 $SG\,+\,SU(2)_1$ | [文献 + 推导] |
| 重子拓扑荷 | $B=\Delta\eta'/(6\pi)$ | [文献] |
| 标准中心扭曲最低权重 | $(0,1/4)$ 或 $(1/4,0)$ | [推导] |
| 最小模型单 soliton 阈值 | $\rho^{(1)}\sim(s-M_B^2)^{-1/2}$ | [条件] |
| 最小缺陷的应力张量扰动 | 红外无关 | [推导：限定算符空间] |
| 微观最低缺陷唯一性 | 尚不能由已知对称性推出 | [待证] |
| 微观核心谱、散射相移与 RG 初值 | 未完成匹配 | [待证] |

**目前最精确的研究陈述：**

> 从带 baryon-'t Hooft flux 的 small-$T^2$ QCD 出发，可以得到具有明确微观零模来源的二维重子候选算符，并构造其非零树级四维源投影。在领先阶 $SG\times SU(2)_1$ 描述中，标准中心扭曲的最低 flavor 权重为 $1/4$；若真实 $B=1$ 红外缺陷由这一最小通道支配，且不存在改变阈值的核心散射及更低态，则单 soliton 的谱密度指数为 $-1/2$。微观缺陷固定点及完整最低谱尚未独立证明。

---

<a id="appendix-a"></a>
## 附录 A：横向零模的显式波函数与非零 Wronskian

在 [1] 所采用的局部规范下，令

$$
X=\frac{x_3}{L},\quad Y=\frac{x_4}{L},\quad
z=X-iY,
$$

可选取规范约定一致的零模形式

$$
\boxed{v^a(y)=\mathcal N_\perp e^{-\pi X^2/3}u_a(z),\qquad
u_a(z)=\sum_{n\in\mathbb Z}
\exp\!\left[-3\pi\left(n+\frac{a-1}{3}\right)^2
+2\pi\left(n+\frac{a-1}{3}\right)z\right].}
$$

相应的背景 twisted boundary conditions 由 clock/shift 矩阵实现；这些 $u_a$ 是局部截面的分量，不能作为全环面的普通周期标量来处理。

将三个横向分离点对应的全纯颜色向量构成 determinant，可以直接验证

$$
\det[\mathbf u(0),\mathbf u(1/3),\mathbf u(2/3)]
\simeq 0.12553202345\ne0,
$$

以及

$$
\det[\mathbf u(0),\mathbf u'(0),\mathbf u''(0)]
\simeq2.42169200583\ne0.
$$

这些值来自对上述**已选定规范与无量纲化的级数**直接求和，不是四维 QCD 格点谱数据。给定相应的公共高斯及 Wilson-line 因子之后，它们证明可选择非零的树级零模颜色系数。

简短复核程序（Python 3 + NumPy）：

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

局域三导数源在环面上仍携带总 $B=1$ 的背景磁通，因此需将其横向系数视为带电截面；若希望定义仅依赖二维坐标的源，可选取同变换性质的测试截面 $w_B(y)$ 做 $\int_{T^2}d^2y\,w_B^*(y)\mathcal J_{4d}(x,y)$。

<a id="appendix-b"></a>
## 附录 B：$U(2)_1\to SG+SU(2)_1$ 的逐项推导

记 $U=e^{i\eta'/2}g$，则

$$
\begin{aligned}
\partial_\mu U&=e^{i\eta'/2}
\left(\partial_\mu g+\frac i2(\partial_\mu\eta')g\right),\\
\partial_\mu U^\dagger&=
\left(\partial_\mu g^\dagger-\frac i2(\partial_\mu\eta')g^\dagger\right)e^{-i\eta'/2}.
\end{aligned}
$$

展开四项后，交叉项的 trace 正比于 $\operatorname{tr}(g^\dagger\partial_\mu g)=0$，而 $\operatorname{tr}(g^\dagger g)=2$，故

$$
\operatorname{tr}(\partial U^\dagger\partial U)
=\operatorname{tr}(\partial g^\dagger\partial g)+\frac12(\partial\eta')^2.
$$

令 $A=g^{-1}dg$、$a=(i/2)d\eta'$，有 $U^{-1}dU=A+a\mathbf1$，且 $a\wedge a=0$：

$$
\operatorname{tr}(A+a\mathbf1)^3
=\operatorname{tr}A^3+3a\wedge\operatorname{tr}(A\wedge A)
=\operatorname{tr}A^3.
$$

最后，由 $\det U=e^{i\eta'}$，可把原文的 vortex 顶点

$$
-e^{i\theta/3}(\det U)^{-1/3}+\text{h.c.}
$$

转成 $-2\cos[(\eta'-\theta)/3]$，并吸收相应的系数至 $\zeta$。全局 $\mathbb Z_3$ 识别不会因局部代数分解而自动消失。

<a id="appendix-c"></a>
## 附录 C：经典 sine-Gordon kink 与涨落谱

采用真空能量已扣除的静态能量泛函

$$
E[\eta']=\int dx\left[
\frac{(\partial_x\eta')^2}{16\pi}
+2\zeta\left(1-\cos\frac{\eta'}3\right)\right].
$$

定义 $m^2=16\pi\zeta/9$，满足 $\Delta\eta'=6\pi$ 的经典解是

$$
\boxed{\eta'_K(x)=12\arctan e^{m(x-X)},\qquad
\partial_x\eta'_K(x)=6m\,\operatorname{sech}[m(x-X)].}
$$

直接积分：

$$
\int dx\,(\partial_x\eta'_K)^2
=36m^2\int dx\,\operatorname{sech}^2[m(x-X)]
=72m.
$$

用一阶积分关系得到经典 kink 质量

$$
\boxed{M_K^{\rm cl}=\frac{1}{8\pi}\,72m=\frac{9m}{\pi}.}
$$

它不是量子 sine-Gordon 的精确 soliton 质量。小涨落满足

$$
\boxed{H_K=-\partial_x^2+m^2\left[1-2\operatorname{sech}^2(m(x-X))\right]
=A^\dagger A,\qquad
A=\partial_x+m\tanh(m(x-X)).}
$$

正规化零模为 $\psi_0\propto\operatorname{sech}(m(x-X))$，对应质心平移；没有其他正规化的离散 shape bound state，连续谱从 $\omega^2=m^2$ 开始。**它仅约束纯 SG 的经典 singlet 涨落，不能排除四维 QCD 的额外复合核心态。**

<a id="appendix-d"></a>
## 附录 D：标准中心扭曲的有限体积能谱

若进一步将剩余空间方向有限化为长度 $R$，则 flavor CFT 能量为

$$
E_f(R)=\frac{2\pi v}{R}
\left(h+\bar h-\frac{c}{12}\right),
\qquad c=1.
$$

标准扭曲最低层 $h+\bar h=1/4$，与未扭曲真空的差为

$$
\boxed{\Delta E_f(R)=\frac{2\pi v}{R}\cdot\frac14
=\frac{\pi v}{2R}.}
$$

在**最小因子化、适当拓扑边界条件、无额外 $1/R$ 缺陷相移贡献**的假设下，可考虑拟合

$$
E_{B=1}(R)-E_{B=0}(R)
=M_B+\frac{\pi v}{2R}+\cdots.
$$

对应 $SU(2)_1$ characters 的低阶展开为

$$
\begin{aligned}
\chi_0(q)&=q^{-1/24}(1+3q+4q^2+7q^3+13q^4+\cdots),\\
\chi_{1/2}(q)&=q^{5/24}(2+2q+6q^2+8q^3+14q^4+\cdots).
\end{aligned}
$$

将两个手征通道合并、令 $q=\bar q$ 进行形式能级计数，得到最低简并度序列

$$
\boxed{d_n=4,\ 16,\ 40,\ 96,\ 204,\ldots}
$$

它仅针对标准扭曲 CFT，不含移动 soliton 质心塔，也不含可能的核心 Hilbert space；它不是四维格点 QCD 数据。

<a id="appendix-e"></a>
## 附录 E：单 soliton 谱密度的相空间推导及归一化说明

对一个手征软模，取

$$
\frac1{z^{1/2}}=\frac1{\sqrt\pi}
\int_0^\infty d\varepsilon\,
\varepsilon^{-1/2}e^{-\varepsilon z}.
$$

设 soliton 的 rapidity 为 $\vartheta$，其动量为

$$
p_{\rm sol}^0=M\cosh\vartheta,
\qquad p_{\rm sol}^1=M\sinh\vartheta.
$$

与一支右移动软模 $p_f=(\varepsilon,\varepsilon)$ 组合，有

$$
\begin{aligned}
P^0&=M\cosh\vartheta+\varepsilon,\\
P^1&=M\sinh\vartheta+\varepsilon,\\
s=P^2&=M^2+2M\varepsilon e^{-\vartheta}.
\end{aligned}
$$

变量变换的 Jacobian 满足

$$
\left|\frac{\partial(P^0,P^1)}
{\partial(\vartheta,\varepsilon)}\right|
=M e^{-\vartheta}=P_-.
$$

取相应拓扑顶点的单 soliton form factor，在本文的左右手性约定及 [3] 的归一化框架内，其 rapidity 权重可写为 $|F_L(\vartheta)|^2\propto e^{-3\vartheta/2}$（右手版本宇称相反）。于是相空间积分中

$$
\frac{|F_L(\vartheta)|^2\,\varepsilon^{-1/2}}{P_-}
\ \propto\ P_-\,(s-M^2)^{-1/2}.
$$

因此在剥除固定的 $P_-$ 运动学因子后，

$$
\boxed{\rho_L^{(1)}(s)=A_L
\frac{\Theta(s-M^2)}{\sqrt{s-M^2}}.}
$$

$A_L$ 包含二维算符归一化、singlet soliton 的 form factor 及四维源匹配系数，不能仅由 $SU(2)_1$ 权重确定。由宇称和对称归一化可得到相应的 $\rho_R^{(1)}$。对不同的谱密度张量分解方式，$P_\pm$ 的提取约定必须保持一致。

<a id="references"></a>
## 参考文献

1. Y. Tanizaki and M. Ünsal, *Center vortex and confinement in Yang–Mills theory and QCD with anomaly-preserving compactifications*, **PTEP 2022**, 04A108, [arXiv:2201.06166](https://arxiv.org/abs/2201.06166), [DOI](https://doi.org/10.1093/ptep/ptac042). —— 原始磁通紧致化背景及零模分析。
2. Y. Hayashi and Y. Tanizaki, *Semiclassics for the QCD vacuum structure through $T^2$-compactification with the baryon-'t Hooft flux*, **JHEP 08 (2024) 001**, [arXiv:2402.04320](https://arxiv.org/abs/2402.04320), [DOI](https://doi.org/10.1007/JHEP08(2024)001). —— 残余 $\mathbb Z_3$、非阿贝尔玻色化、扩展的 $\eta'$ 周期和真空有效作用量。
3. S. Lukyanov and A. B. Zamolodchikov, *Form factors of soliton-creating operators in the sine-Gordon model*, **Nucl. Phys. B 607 (2001) 437–455**, [arXiv:hep-th/0102079](https://arxiv.org/abs/hep-th/0102079), [DOI](https://doi.org/10.1016/S0550-3213(01)00262-0). —— soliton-creating vertex 的 form-factor 方法。

---

*说明：本文区分了原始文献直接给出的理论结构与后续在指定模型内完成的推导。尚未完成的四维微观低能谱匹配不应在引用本文时省略。*
