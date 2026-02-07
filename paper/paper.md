---
title: The Acceleration Principle and the Nature of Business Cycles
authors:
  - name: Gregory C. Chow
    affiliations:
      - Thomas J. Watson Research Center, IBM, Yorktown Heights, New York
date: 1968-08-01
venue: The Quarterly Journal of Economics, Vol. 82, No. 3 (Aug., 1968), pp. 403–418
bibliography: references.bib
acknowledgments: >
  A preliminary version of this paper was presented before the Joint Faculty Colloquium
  on Mathematical Economics and Econometrics of Columbia, Johns Hopkins, University of
  Pennsylvania and Princeton, held at Columbia University in May 1966. Parts of this paper
  were written while the author was visiting the Harvard Economics Department and were
  presented to the Research Seminar on Quantitative and Mathematical Economics there,
  and to the Econometrics Seminar at MIT in May 1967. All comments are gratefully
  acknowledged. The author has also benefited greatly from the suggestions of T. W. Anderson,
  Alan J. Hoffman, and Richard E. Levitan.
---

+++ {"part": "abstract"}
I. Introduction, 403. — II. Demand equations and evidence for acceleration, 404. — III. The nonstochastic case: no oscillations without acceleration, 406. — IV. Autocovariances of a linear stochastic system, 408. — V. Spectral densities of a linear stochastic system, 411. — VI. Conclusions, 417.
+++

(sec-introduction)=
## I. Introduction

Half a century ago, J. M. Clark stressed the importance of the acceleration principle in business cycle theory.[^fn1] Almost thirty years ago P. A. Samuelson pointed out that the acceleration relation can interact with the multiplier to generate oscillations in national income.[^fn2] This paper presents a formulation of the acceleration principle and some strong supporting evidence. It attempts to ascertain whether the acceleration principle is necessary for the generation of oscillations in national output. It also extends the discussion of the nature of economic fluctuations from the nonstochastic to the stochastic case.

[^fn1]: J. M. Clark, "Business Acceleration and the Law of Demand: A Technical Factor in Economic Cycles," *Journal of Political Economy*, XXV (Mar. 1917), 217–35. {cite}`clark1917`

[^fn2]: P. A. Samuelson, "Interactions between the Multiplier Analysis and the Principle of Acceleration," *Review of Economic Statistics*, XXI (May 1939), 75–78. {cite}`samuelson1939`

Recently I constructed a simple macroeconometric model of the United States economy in the form of a system of linear stochastic difference equations in which the acceleration principle plays an important role.[^fn3] The present paper is partly the outcome of an analytical study of the dynamic properties of such a linear stochastic system. The tools employed are the autocovariances and the spectral densities of the time series so generated. The presentation of results on these matters will be elementary and self-contained.

[^fn3]: G. C. Chow, "Multiplier, Accelerator, and Liquidity Preference in the Determination of National Income in the United States," *Review of Economics and Statistics*, XLIX (Feb. 1967), 1–15. {cite}`chow1967`

This paper begins with a formulation of the acceleration principle and its supporting evidence in {ref}`sec-demand-equations`. {ref}`sec-nonstochastic` shows that, without an acceleration equation, a system of nonstochastic linear demand equations for the components of national output cannot produce oscillations in the variables. This amounts to showing that the characteristic roots of the system are all real and positive. The discussion is generalized to allow for random disturbances in the equations. In {ref}`sec-autocovariances` and {ref}`sec-spectral-densities`, respectively, the autocovariance matrix and the spectral density matrix will be derived in an elementary fashion. It is shown that random shocks, when introduced into an otherwise nonoscillatory system, can generate cycles. Thus the acceleration principle is no longer necessary. While {ref}`sec-autocovariances` and {ref}`sec-spectral-densities` are confined to the stationary case (with all roots less than one in absolute value), {ref}`sec-conclusions` contains brief comments on the nonstationary case as well as some concluding remarks on the nature of business cycles.

(sec-demand-equations)=
## II. Demand Equations and Evidence for Acceleration

To ascertain whether a system of nonstochastic economic equations can produce oscillations without acceleration, one obviously has to specify the nature of the equations. It seems relevant to restrict the equations in a macroeconomic model to demand equations for different components $y_i$ of national product $Y = \sum y_i$ which obey simple distributed lags:[^fn4]

[^fn4]: The intercept will be omitted, as exogenous variables are omitted in this paper which treats business cycles as the result of interactions of endogenous forces, holding the exogenous variables constant.

$$
y_{it} = a_i Y_t + b_i y_{i, t-1}.
$$ (eq-1)

Of course, demand equations for investment goods and for some consumer durables are not of this type because of acceleration, but our purpose is precisely to find out whether there could be oscillations if all demand equations were of the form {eq}`eq-1`. In other words, while Samuelson[^fn5] demonstrated that the interaction of the multiplier and the accelerator can produce oscillations, we ask whether the latter is necessary, in the context of a system of equations.

[^fn5]: {cite}`samuelson1939`.

For investment goods and possibly consumer durables, the demand functions for total stock $s_i$ are assumed to be of the same form:

$$
s_{it} = a_i Y_t + b_i s_{i, t-1}.
$$ (eq-2)

The flow of net investment $y_{it}^n$ is $\Delta s_{it} = s_{it} - s_{i, t-1}$:

$$
y_{it}^n = \Delta s_{it} = a_i \Delta Y_t + b_i y_{i, t-1}^n
$$ (eq-3)

which is our formulation of the acceleration principle. If one chooses to work with gross investment $y_{it} = \Delta s_{it} + \delta_i s_{i, t-1} = s_{it} - (1 - \delta_i) s_{i, t-1}$ where $\delta_i$ is the percentage rate of depreciation, the demand equation will be

$$
y_{it} = a_i \Delta Y_t + a_i \delta_i Y_{t-1} + b_i y_{i, t-1} = a_i [Y_t - (1 - \delta_i) Y_{t-1}] + b_i y_{i, t-1}.
$$ (eq-4)

In the previous macroeconometric study, I tested equation {eq}`eq-4` using annual observations (1931–40 and 1948–63) on new construction, on gross private domestic investment in producers' durable equipment combined with change in business inventories, and on the last two variables separately, the $Y$ variable being gross national product minus taxes net of transfers.[^fn6] In each case, the coefficient of $Y_{t-1}$ turned out to be of opposite sign, and slightly smaller in absolute value, as compared with the coefficient of $Y_t$. In other words, when $\Delta Y_t$ and $Y_{t-1}$ were used, the coefficient of the latter turned out to be a small fraction of the coefficient of the former.

[^fn6]: {cite}`chow1967`.

Using annual data (1922–41 and 1948–57) on net investment in automobiles obtained in previous work,[^fn7] I have found, by the method of least squares,

[^fn7]: G. C. Chow, *Demand for Automobiles in the United States* (Amsterdam: North-Holland Publishing Co., 1957), and "Statistical Demand Functions for Automobiles and Their Use for Forecasting," in A. C. Harberger, ed., *Demand for Durable Goods* (Chicago: University of Chicago Press, 1960). {cite}`chow1957,chow1960`

$$
y_t^n = \underset{(.0022)}{.0155} Y_t - \underset{(.0020)}{.0144} Y_{t-1} - \underset{(.0056)}{.0239} p_t + \underset{(.0040)}{.0199} p_{t-1} + \underset{(.101)}{.351} y_{t-1}^n + \text{const.}
$$ (eq-5)

where $Y_t$ is real disposable personal income per capita, $p_t$ is a relative price index for automobiles, and $y_t^n$ is per capita net investment in passenger automobiles. Here again, the coefficients of $Y_{t-1}$ and $p_{t-1}$ are practically the negatives of the coefficients of $Y_t$ and $p_t$.

The strong empirical support for the acceleration principle as formulated in equations {eq}`eq-3` and {eq}`eq-4` should not be surprising to those willing to accept the stock adjustment equation {eq}`eq-2`, as {eq}`eq-3` and {eq}`eq-4` are the results of differencing {eq}`eq-2`. In earlier work,[^fn8] I presented demand functions for automobile stock in the form of equation {eq}`eq-2`, and for the purchase of new automobiles by subtracting $(1 - \delta) s_{i, t-1}$ from both sides of {eq}`eq-2` while keeping $s_{i, t-1}$ as an explanatory variable; the price variable $p_t$ was used in addition to $Y_t$ in the stock adjustment equation. The calculation presented in equation {eq}`eq-5` is essentially the first difference of {eq}`eq-2`, rather than the result of subtracting $(1 - \delta) s_{i, t-1}$ from both sides.

[^fn8]: {cite}`chow1967`.

(sec-nonstochastic)=
## III. The Nonstochastic Case: No Oscillations Without Acceleration

To set the stage for later analyses of the cyclical properties of a system of linear difference equations, with or without acceleration, write the nonstochastic system as

$$
y_t = A y_{t-1}
$$ (eq-6)

where $y_t$ is a $p$-component column vector of dependent variables at time $t$, and $A$ is a $p$ by $p$ matrix of coefficients. Any higher order system to start with is understood to have been reduced to first order by redefining variables. This paper is confined to the interactions of endogenous variables, leaving out the possible effects of exogenous variables.

Let $\lambda_1, \lambda_2, \ldots, \lambda_p$ be the characteristic roots of $A$, assumed to be distinct, $D_\lambda$ the diagonal matrix with these roots on the diagonal, and $B = (b_{ij})$ the matrix whose columns are the (right) characteristic vectors corresponding to these roots:

$$
AB = B D_\lambda \quad \text{or} \quad A = B D_\lambda B^{-1}.
$$ (eq-7)

If the initial values $y_0$ at time 0 are given, the solution of {eq}`eq-6` is

$$
y_t = A^t y_0 = B D_\lambda^t B^{-1} y_0.
$$ (eq-8)

The solution {eq}`eq-8` can be interpreted in terms of a set of canonical variables $z_t = B^{-1} y_t$ that are linear combinations of the original variables:

$$
z_t = B^{-1} y_t = B^{-1} A y_{t-1} = D_\lambda B^{-1} y_{t-1} = D_\lambda z_{t-1}.
$$ (eq-9)

The solution for the $i$-th canonical variable is $z_{it} = z_{i0} \lambda_i^t$. The solutions for the original variables $y_t = B z_t$ are thus the same linear combination $B$ of the solutions $z_{it} = z_{i0} \lambda_i^t$:

$$
y_t = B z_t = B D_\lambda^t z_0
$$ (eq-10)

as we have in {eq}`eq-8`. The components of {eq}`eq-10` are

$$
y_{it} = b_{i1} z_{10} \lambda_1^t + b_{i2} z_{20} \lambda_2^t + \cdots + b_{ip} z_{p0} \lambda_p^t \qquad (i = 1, \ldots, p)
$$ (eq-11)

which are linear combinations of $\lambda_j^t$ $(j = 1, \ldots, p)$. If the roots $\lambda_j$ are all real and positive, there will be no prolonged oscillations in the solution {eq}`eq-11`. With only real and positive roots, some negative coefficients $b_{ij} z_{j0}$ could produce a few swings in the time path {eq}`eq-11` initially, but the solution will soon behave like an exponential function according to the largest root.

Returning to our problem of a system of demand equations {eq}`eq-1` without acceleration,

$$
\begin{bmatrix}
1 - a_1 & -a_1 & -a_1 & \cdots & -a_1 \\
-a_2 & 1 - a_2 & -a_2 & \cdots & -a_2 \\
\vdots & & \ddots & & \vdots \\
-a_p & -a_p & -a_p & \cdots & 1 - a_p
\end{bmatrix}
\begin{bmatrix}
y_{1t} \\ y_{2t} \\ \vdots \\ y_{pt}
\end{bmatrix}
=
\begin{bmatrix}
b_1 & & 0 \\
& b_2 & \\
& & \ddots & \\
0 & & & b_p
\end{bmatrix}
\begin{bmatrix}
y_{1, t-1} \\ y_{2, t-1} \\ \vdots \\ y_{p, t-1}
\end{bmatrix}
$$ (eq-12)

or

```{math}
:enumerated: false
G y_t = D_b y_{t-1},
```

we inquire whether, and under what conditions, the roots of $A = G^{-1} D_b$ will all be real and positive, assuming that the coefficients $a_i$ and $b_i$ are real and positive. First to be established is the nonsingularity of $G$. This is done by evaluating the roots of $G$.[^fn9] Write $G = I - F$, where the $i$-th row of $F$ is $(a_i, a_i, \ldots, a_i)$. $F$ has rank one, and hence only one nonzero root. This root is $\sum_{i=1}^{p} a_i$, as it can be easily checked. The roots of $G$ satisfy $|G - \mu I| = 0$ or $|F - (1 - \mu)I| = 0$, and are equal to one minus the roots of $F$, i.e., $1 - \sum a_i, 1, \ldots, 1$. Thus, $G$ is nonsingular if and only if $\sum a_i \neq 1$.

[^fn9]: This argument is due to A. J. Hoffman.

The main results are, first, that the roots of system {eq}`eq-12` are all real; and, second, they are all positive if and only if the sum $\sum_{j=1}^{p} a_j$ of the marginal propensities is less than unity.

To show that the roots of $A$ are real, consider $A^{-1} = D_b^{-1} G$. Let $D_a$ be the diagonal matrix with $a_1, \ldots, a_p$ on its diagonal. $D_b^{-1} G = (D_b^{-1} D_a)(D_a^{-1} G)$ is the product of two real symmetric matrices, the former $D_b^{-1} D_a$ being positive definite. Therefore, the roots of $D_b^{-1} G$, and of $G^{-1} D_b$, are all real.[^fn10]

[^fn10]: See, for example, R. Bellman, *Introduction to Matrix Analysis* (New York: McGraw-Hill, 1960), p. 36, Exercise 4. {cite}`bellman1960`

To obtain a necessary and sufficient condition for all positive roots, observe that the roots of $D_b^{-1} G$ can be obtained from the following equivalent characteristic equations:

```{math}
:enumerated: false
\begin{aligned}
|D_b^{-1} G - \mu I| &= 0 \\
|D_b^{-1/2} G D_b^{-1/2} - \mu I| &= 0 \\
|D_b^{-1/2} D_a^{1/2} (D_a^{-1} G) D_a^{1/2} D_b^{-1/2} - \mu I| &= 0.
\end{aligned}
```

Therefore, they are the same as the roots of the last symmetric matrix. The latter roots are all positive if and only if the roots of the symmetric matrix $D_a^{1/2}(D_a^{-1} G) D_a^{1/2}$ are; but the roots of $D_a^{1/2} (D_a^{-1} G) D_a^{1/2}$ are indeed those of $G$. As we have evaluated, the roots of $G$ are all positive if and only if $1 - \sum a_i$ is positive.

It has been shown that the solution of system {eq}`eq-12` cannot oscillate, under the assumption $\sum_{j=1}^{p} a_j < 1$. By a numerical example, of two variables say, one can easily demonstrate that, if a demand equation {eq}`eq-1` is replaced by an acceleration equation {eq}`eq-3` or {eq}`eq-4` in the system {eq}`eq-12`, complex roots can be generated.

(sec-autocovariances)=
## IV. Autocovariances of a Linear Stochastic System

To generalize our discussion to the stochastic case is important not only for the study of dynamic properties of linear econometric models, but for business cycle theory. In the words of {cite}`frisch1933`:

> The examples we have discussed . . . show that when an [deterministic] economic system gives rise to oscillations, these will most frequently be damped. But in reality the cycles . . . are generally not damped. How can the maintenance of the swings be explained? . . . One way which I believe is particularly fruitful and promising is to study what would become of the solution of a determinate dynamic system if it were exposed to a stream of erratic shocks . . .
>
> Thus, by connecting the two ideas: (1) the continuous solution of a determinate dynamic system and (2) the discontinuous shocks intervening and supplying the energy that may maintain the swings — we get a theoretical setup which seems to furnish a rational interpretation of those movements which we have been accustomed to see in our statistical time data.[^fn11]

[^fn11]: Ragnar Frisch, "Propagation Problems and Impulse Problems in Dynamic Economics," *Economic Essays in Honour of Gustav Cassel* (London: Allen & Unwin, 1933), pp. 197 and 202–3.

It turns out that oscillations in the deterministic system are neither necessary nor sufficient in producing "cycles" in the stochastic system, but the importance of the stochastic element should be stressed.

In the stochastic case, we add a random vector $u_t$ to the right side of system {eq}`eq-6`:

$$
y_t = A y_{t-1} + u_t
$$ (eq-13)

with $E u_t = 0$, $E u_t u_t' = V$, and $E u_t u_{t-k}' = 0$ for $k \neq 0$. It is further assumed that the roots of $A$ are all smaller than one in absolute value, so that[^fn12] the covariances $\gamma_{ij, k} = E y_{it} y_{j, t-k}$ exist and are independent of $t$, leaving a brief discussion of the nonstationary case (with some roots of $A$ greater than one) to {ref}`sec-conclusions`. The covariances $\gamma_{ij, k}$ do provide information about the dynamic properties of the system. For example, if $\gamma_{ii, k}$ is an "approximately" periodic function of the lag $k$, with forty months as the length of the period, say, then observations on the time series $y_{it}$ made forty months apart are more highly correlated than those made at other intervals — the sense in which a forty-month cycle can be claimed for $y_{it}$ will be further specified by the spectral density function of $y_{it}$, to be derived in {ref}`sec-spectral-densities`.

[^fn12]: A proof will be provided following equation {eq}`eq-18`.

It is quite straightforward to derive the autocovariance matrix[^fn13]

[^fn13]: Many results on the autocovariance matrix can be found, for example, in M. H. Quenouille, *The Analysis of Multiple Time-Series* (London: Charles Griffin, 1957). {cite}`quenouille1957`

$$
\Gamma_k = E y_t y_{t-k}' = (\gamma_{ij, k}) = \Gamma_{-k}'
$$ (eq-14)

in terms of the parameters $A$ and $V$ of the system {eq}`eq-13`. Postmultiply each term of {eq}`eq-13` by $y_{t-k}'$, and take expectation:

$$
E y_t y_{t-k}' = A E y_{t-1} y_{t-k}' + E u_t y_{t-k}'.
$$ (eq-15)

For $k = 0$, the last term is $V$, and for $k = 1, 2, \ldots$, the last term is $0$. Note also that $\Gamma_{-1} = \Gamma_1'$. Hence, {eq}`eq-15` can be written as

$$
\Gamma_0 = A \Gamma_{-1} + V = A \Gamma_1' + V, \quad \text{and}
$$ (eq-16)

$$
\Gamma_k = A \Gamma_{k-1} \qquad (k = 1, 2, 3, \ldots).
$$ (eq-17)

Once $\Gamma_0$ (the covariance matrix of $y_t$) is known, {eq}`eq-17` can be used to find $\Gamma_k$ $(k = 1, 2, \ldots)$, i.e., $\Gamma_k = A^k \Gamma_0$.

To find $\Gamma_0$, we use {eq}`eq-16` to iterate, noting $\Gamma_1 = A \Gamma_0$ and $\Gamma_1' = \Gamma_0 A'$:

$$
\Gamma_0 = V + A \Gamma_1' = V + A \Gamma_0 A' = V + A(V + A \Gamma_0 A') A' = V + A V A' + A^2 V A'^2 + \cdots
$$ (eq-18)

From {eq}`eq-18`, we will observe that $\Gamma_0$ exists if the roots of $A$ are all less than one in absolute value. Using {eq}`eq-7` and letting $W = (w_{ij}) = B^{-1} V B'^{-1}$ be the symmetric positive semidefinite matrix, we write {eq}`eq-18` as

$$
\Gamma_0 = \sum_{s=0}^{\infty} A^s V A'^s = \sum_{s=0}^{\infty} B D_\lambda^s B^{-1} V B'^{-1} D_\lambda^s B' = B \left( \sum_{s=0}^{\infty} w_{ij} \lambda_i^s \lambda_j^s \right) B'.
$$ (eq-19)

Hence, the matrix in parentheses exists if all the roots are less than one in absolute value. Assuming this condition to hold, we can write out the autocovariance matrices explicitly:

$$
\Gamma_0 = B \left( \frac{w_{ij}}{1 - \lambda_i \lambda_j} \right) B'
$$ (eq-20)

$$
\Gamma_k = A^k \Gamma_0 = B D_\lambda^k B^{-1} \Gamma_0 = B D_\lambda^k \left( \frac{w_{ij}}{1 - \lambda_i \lambda_j} \right) B'.
$$ (eq-21)

It is useful to interpret {eq}`eq-21` in terms of the canonical variables $z_t = B^{-1} y_t$. Premultiplying {eq}`eq-13` by $B^{-1}$ shows that the canonical variables satisfy

$$
z_t = D_\lambda z_{t-1} + B^{-1} u_t = D_\lambda z_{t-1} + \epsilon_t.
$$ (eq-22)

The covariance matrix of the residuals $\epsilon_t$ is

$$
E \epsilon_t \epsilon_t' = E B^{-1} u_t u_t' B'^{-1} = B^{-1} V B'^{-1} = W
$$ (eq-23)

where the matrix $W$ has been previously defined. Analogous to {eq}`eq-17` and {eq}`eq-19`, the autocovariance matrix of $z_t$, denoted by $\Gamma_k^*$, satisfies the relations

$$
\Gamma_k^* = D_\lambda \Gamma_{k-1}^* = D_\lambda^k \Gamma_0^* \qquad (k = 1, 2, 3, \ldots)
$$ (eq-24)

and

$$
\Gamma_0^* = \sum_{s=0}^{\infty} D_\lambda^s W D_\lambda^s = \left( \sum_{s=0}^{\infty} w_{ij} \lambda_i^s \lambda_j^s \right) = \left( \frac{w_{ij}}{1 - \lambda_i \lambda_j} \right).
$$ (eq-25)

The relation between $\Gamma_k$ and $\Gamma_k^*$ is

$$
\Gamma_k = E y_t y_{t-k}' = E B z_t z_{t-k}' B' = B \Gamma_k^* B' \quad \text{or} \quad \Gamma_k = B D_\lambda^k \Gamma_0^* B' \qquad (k = 0, 1, 2, \ldots)
$$ (eq-26)

which is the same as {eq}`eq-21`.

By {eq}`eq-24`, each covariance $\gamma_{mn, k}^*$ of the canonical variables is $\gamma_{mn, 0}^* \lambda_m^k$. By {eq}`eq-26`, the covariance $\gamma_{ij, k}$ of the original variables is a linear combination of $\lambda_m^k$:

$$
\gamma_{ij, k} = \sum_m \sum_n b_{im} b_{jn} \gamma_{mn, k}^* = \sum_m b_{im} \left( \sum_n b_{jn} \gamma_{mn, 0}^* \right) \lambda_m^k = \sum_m d_{ij, m} \lambda_m^k \qquad (k = 0, 1, 2, \ldots)
$$ (eq-27)

and

```{math}
:enumerated: false
\gamma_{ij, -k} = \gamma_{ji, k} = \sum_m d_{ji, m} \lambda_m^k \qquad (k = 1, 2, 3, \ldots).
```

Comparing the covariance function {eq}`eq-27` and the time path {eq}`eq-11` of the nonstochastic model, we see a formal resemblance: both are linear combinations of $\lambda_m^k$. In the nonstochastic case, the coefficients of {eq}`eq-11` depend on the initial values $y_{i0}$, or on the initial values $z_{i0}$ and $b_{ij}$. In the stochastic case, the coefficients of {eq}`eq-27` depend on the covariances $\gamma_{ij, 0}$, or, in terms of canonical variables, on $\gamma_{ij, 0}^*$ and $b_{ij}$.

If complex roots exist, they come in conjugate pairs. The contribution of a pair of complex roots to the linear combination {eq}`eq-27` can be simply stated. Let the pair be

$$
\lambda_1 = r e^{i\theta}, \quad \lambda_2 = r e^{-i\theta} \qquad (i = \sqrt{-1}).
$$ (eq-28)

Their contribution to $\gamma_{ij, k}$ is

$$
d_{ij, 1} r^k e^{i\theta k} + d_{ij, 2} r^k e^{-i\theta k}.
$$ (eq-29)

If this contribution is real, we let the coefficients $d_{ij, 1}$ and $d_{ij, 2}$ be conjugate complex, say,

$$
d_{ij, 1} = s e^{i\rho}, \quad d_{ij, 2} = s e^{-i\rho}.
$$ (eq-30)

Substituting {eq}`eq-30` into {eq}`eq-29` gives

$$
s r^k (e^{i(\theta k + \rho)} + e^{-i(\theta k + \rho)}) = 2 s r^k \cos(\theta k + \rho).
$$ (eq-31)

Thus, with the absolute value $r$ of the roots less than one, the contribution {eq}`eq-31` to $\gamma_{ij, k}$ is a damped cosine function of $k$, with frequency $\theta$. In the nonstochastic model, the complex roots {eq}`eq-28` would generate a component of the time path which is a damped cosine function of $t$, with the same frequency $\theta$, but the phase would in general be different from $\rho$.

Damped oscillations in (a component of) the time path in the nonstochastic model, due to a pair of complex roots, will necessarily be associated with damped oscillations in (a component of) the autocovariance function $\gamma_{ii, k}$. It is in this sense that the former oscillations could be maintained in the stochastic model. The interesting questions are whether damped oscillations in the deterministic model are necessary, and sufficient, to generate distinct "cycles" in the stochastic time series in the sense of their spectral densities. We will turn to this subject in the next section.

(sec-spectral-densities)=
## V. Spectral Densities of a Linear Stochastic System[^fn14]

[^fn14]: For a discussion of spectral densities, see, for example, D. R. Cox and H. D. Miller, *The Theory of Stochastic Processes* (New York: Wiley, 1965), Chap. 8, and P. Whittle, *Prediction and Regulation by Linear Least-Square Methods* (New York: D. Van Nostrand, 1963), Chap. 2. {cite}`cox1965,whittle1963`

There are certainly many interesting aspects of business cycles, but this paper is confined mainly to their periodicities. For this purpose, the spectral density is a useful tool. Before going into the periodicities in the relations among time series, it is well to begin with the periodicities of an individual time series $y_{it}$. The spectral density of a discrete time series $y_{it}$ is a weighted sum of its autocovariance function (omitting a normalization constant),

$$
f_{ii}(\omega) = \sum_{k=-\infty}^{\infty} \gamma_{ii, k} \cos \omega k
$$ (eq-32)

where the weights $\cos \omega k$ are periodic, with frequency $\omega$ (or with period length $2\pi / \omega$). Intuitively speaking, if the autocovariance function $\gamma_{ii, k}$ happens to be approximately periodic with frequency $\theta$ (or period length $2\pi / \theta$), then weighing it by a periodic function $\cos \theta k$ with the same frequency will give a large sum, i.e., $f_{ii}(\omega)$ will be large for $\omega = \theta$. For a discrete time series, the shortest cycle that can be detected is of length 2, i.e., with frequency $\pi$. Thus, the range of $\omega$ for the spectral density $f_{ii}(\omega)$ is from $0$ to $\pi$, indicating the strength of the very long cycles and two-period cycles respectively.

The periodic weighing function $\cos \omega k$ is appropriate only for the autocovariance function $\gamma_{ii, k}$ since both have a maximum at $k = 0$, and there is no question of being out of phase. For a cross-covariance function $\gamma_{ij, k}$, which may not have a maximum at $k = 0$, the phase problem in the weighing function arises, and the function

$$
\cos(\omega k + \psi) = (\cos \psi) \cos \omega k - (\sin \psi) \sin \omega k
$$ (eq-33)

for some phase $\psi$ may be appropriate. This suggests using the weighing function

$$
e^{-i\omega k} = \cos \omega k - i \sin \omega k
$$ (eq-34)

which contains the two components $\cos \omega k$ and $\sin \omega k$. For the autocovariance function $\gamma_{ii, k} = \gamma_{ii, -k}$,

$$
\sum_{k=-\infty}^{\infty} \gamma_{ii, k} e^{-i\omega k} = \sum_{k=-\infty}^{\infty} \gamma_{ii, k} \cos \omega k = f_{ii}(\omega)
$$ (eq-35)

since $\sin(-\omega k) = -\sin \omega k$. Using $e^{-i\omega k}$ rather than $\cos \omega k$ as the weighing function will also simplify algebra.

The spectral density matrix is defined as

$$
F(\omega) = \sum_{k=-\infty}^{\infty} \Gamma_k e^{-i\omega k}
$$ (eq-36)

where the diagonal elements are the spectral densities of the individual time series, and the off-diagonal elements are the cross-spectral densities. Although the cross-spectral densities will also be derived, our discussion will be mainly confined to the spectral densities. To evaluate {eq}`eq-36`, we will first evaluate the spectral density matrix $F^*(\omega)$ of the canonical variables which is related to $F(\omega)$ by

$$
F(\omega) = \sum_{k=-\infty}^{\infty} B \Gamma_k^* B' e^{-i\omega k} = B \sum_{k=-\infty}^{\infty} \Gamma_k^* e^{-i\omega k} \; B' = B F^*(\omega) B'
$$ (eq-37)

in view of the relation {eq}`eq-26`.

By {eq}`eq-24` and {eq}`eq-25`, the spectral density matrix of the canonical variables is

$$
\begin{aligned}
F^*(\omega) &= \sum_{k=0}^{\infty} \Gamma_k^* e^{-i\omega k} + \sum_{k=0}^{\infty} \Gamma_{-k}^* e^{i\omega k} - \Gamma_0^* \\
&= \sum_{k=0}^{\infty} D_\lambda^k \Gamma_0^* e^{-i\omega k} + \sum_{k=0}^{\infty} \Gamma_0^* D_\lambda^k e^{i\omega k} - \Gamma_0^* \\
&= \left[ \left( \frac{1}{1 - \lambda_i e^{-i\omega}} + \frac{1}{1 - \lambda_j e^{i\omega}} - 1 \right) \gamma_{ij, 0}^* \right] \\
&= \left[ \frac{1 - \lambda_i \lambda_j}{(1 - \lambda_i e^{-i\omega})(1 - \lambda_j e^{i\omega})} \cdot \frac{w_{ij}}{1 - \lambda_i \lambda_j} \right] \\
&= \left[ \frac{w_{ij}}{(1 - \lambda_i e^{-i\omega})(1 - \lambda_j e^{i\omega})} \right].
\end{aligned}
$$ (eq-38)

With $F^*(\omega)$ in {eq}`eq-37` so substituted, the spectral density matrix of the original variables is

$$
F(\omega) = B \left[ \frac{w_{ij}}{(1 - \lambda_i e^{-i\omega})(1 - \lambda_j e^{i\omega})} \right] B'.
$$ (eq-39)

While the result {eq}`eq-39` gives the entire spectral density matrix, the diagonal elements are of special interest and can be expressed in an alternative way. Let $b_m$ be the $m$-th row of $B$.

$$
f_{mm}(\omega) = b_m F^*(\omega) b_m' = \tfrac{1}{2} b_m [f_{ij}^*(\omega) + f_{ji}^*(\omega)] b_m'.
$$ (eq-40)

Using the expression after the third equality sign in {eq}`eq-38` for $f_{ij}^*(\omega)$,

$$
\begin{aligned}
\bigl[f_{ij}^*(\omega) + f_{ji}^*(\omega)\bigr]
&= \left[ \left( \frac{1}{1 - \lambda_i e^{-i\omega}} + \frac{1}{1 - \lambda_j e^{i\omega}} + \frac{1}{1 - \lambda_j e^{-i\omega}} + \frac{1}{1 - \lambda_i e^{i\omega}} - 2 \right) \gamma_{ij, 0}^* \right] \\
&= \left[ \frac{1 - \lambda_i^2}{(1 - \lambda_i e^{-i\omega})(1 - \lambda_i e^{i\omega})} \gamma_{ij, 0}^* + \frac{1 - \lambda_j^2}{(1 - \lambda_j e^{-i\omega})(1 - \lambda_j e^{i\omega})} \gamma_{ij, 0}^* \right].
\end{aligned}
$$ (eq-41)

Define

$$
g_i = \frac{1 - \lambda_i^2}{(1 - \lambda_i e^{-i\omega})(1 - \lambda_i e^{i\omega})} = \frac{1 - \lambda_i^2}{1 + \lambda_i^2 - 2\lambda_i \cos \omega}
$$ (eq-42)

and let $D_g$ be the diagonal matrix with $g_i$ as its $i$-th diagonal element. Then {eq}`eq-41` becomes

$$
[f_{ij}^*(\omega) + f_{ji}^*(\omega)] = [g_i \gamma_{ij, 0}^* + g_j \gamma_{ij, 0}^*]
$$ (eq-43)

and the spectral density {eq}`eq-40` can be written as

$$
f_{mm}(\omega) = b_m D_g \Gamma_0^* b_m'.
$$ (eq-44)

Observe that {eq}`eq-44` is a linear combination of $g_i$, and that, by {eq}`eq-43`, $g_i$ is proportional to the spectral density

$$
f_{ii}^*(\omega) = \gamma_{ii, 0}^* g_i
$$ (eq-45)

of the $i$-th canonical variable. Therefore, $f_{mm}(\omega)$ is a linear combination of $f_{ii}^*(\omega)$, $i = 1, \ldots, p$.

There is a striking resemblance between {eq}`eq-44` and the $m$th diagonal element of {eq}`eq-26`, i.e.,

$$
\gamma_{mm, k} = b_m D_\lambda^k \Gamma_0^* b_m' = \sum_i d_{mm, i} \lambda_i^k.
$$ (eq-46)

$g_i$ in the former replaces $\lambda_i^k$ in the latter. Thus, whereas the autocovariance function is a linear combination of $\lambda_i^k$, the spectral density function is the same linear combination of $g_i$. This result is expected because we could have obtained $f_{mm}(\omega)$ directly as a weighted sum (over $k$) of {eq}`eq-46`; the weighted summation could be performed on each $\lambda_i^k$,

$$
\sum_{k=0}^{\infty} \lambda_i^k e^{-i\omega k} + \sum_{k=0}^{\infty} \lambda_i^k e^{i\omega k} - 1 = \frac{1}{1 - \lambda_i e^{-i\omega}} + \frac{1}{1 - \lambda_i e^{i\omega}} - 1
$$ (eq-47)

yielding $g_i$.

Once the spectral density has been expressed in terms of the roots, it is convenient to discuss the relationships between prolonged oscillations in the deterministic model (generated by complex roots) and distinct cycles in the stochastic model (defined by a peak of the spectral density function). Are complex roots necessary or sufficient for generating a peak in the spectral density?

To answer this question, the well-known Hansen–Samuelson multiplier-accelerator model will first be used as an example.[^fn15] The second-order stochastic difference equation is written as a first-order system:

[^fn15]: {cite}`samuelson1939`.

$$
\begin{bmatrix} y_{1t} \\ y_{2t} \end{bmatrix}
=
\begin{bmatrix} a_{11} & a_{12} \\ 1 & 0 \end{bmatrix}
\begin{bmatrix} y_{1, t-1} \\ y_{2, t-1} \end{bmatrix}
+
\begin{bmatrix} u_{1t} \\ 0 \end{bmatrix}.
$$ (eq-48)

Since, for this system, $y_{2t}$ is simply $y_{1, t-1}$, we have

$$
\gamma_{11, k} = \gamma_{22, k} = \gamma_{12, k-1} = \gamma_{21, k+1}
$$ (eq-49)

which, when substituted into the homogeneous system {eq}`eq-17`, gives

$$
\begin{bmatrix} \gamma_{12, k-1} & \gamma_{12, k} \\ \gamma_{11, k-1} & \gamma_{11, k} \end{bmatrix}
= A
\begin{bmatrix} \gamma_{12, k-2} & \gamma_{12, k-1} \\ \gamma_{11, k-2} & \gamma_{11, k-1} \end{bmatrix}
\qquad (k = 1, 2, 3, \ldots).
$$ (eq-50)

{eq}`eq-50` implies that, for $k = 1$,

$$
\begin{bmatrix} \gamma_{12, 0} \\ \gamma_{11, 0} \end{bmatrix}
= A
\begin{bmatrix} \gamma_{12, -1} \\ \gamma_{11, -1} \end{bmatrix}.
$$ (eq-51)

The solution for $\gamma_{11, k}$ is, by {eq}`eq-27`,

$$
\gamma_{11, k} = d_{11, 1} \lambda_1^k + d_{11, 2} \lambda_2^k \qquad (k = 0, 1, 2, \ldots)
$$ (eq-52)

which, in view of {eq}`eq-51`, is also valid for $k = -1$. Therefore,

$$
\gamma_{11, -1} = d_{11, 1} \lambda_1^{-1} + d_{11, 2} \lambda_2^{-1} = \gamma_{11, 1} = d_{11, 1} \lambda_1 + d_{11, 2} \lambda_2.
$$ (eq-53)

The condition {eq}`eq-53` will be used to simplify the spectral density function.

As given by equation {eq}`eq-44`, the spectral density function is

$$
\begin{aligned}
f_{11}(\omega) &= d_{11, 1} g_1 + d_{11, 2} g_2 \\
&= \frac{d_{11, 1}(1 - \lambda_1^2)}{1 + \lambda_1^2 - 2\lambda_1 \cos \omega} + \frac{d_{11, 2}(1 - \lambda_2^2)}{1 + \lambda_2^2 - 2\lambda_2 \cos \omega} \\
&= \frac{d_{11, 1}(1 - \lambda_1^2)(1 + \lambda_2^2 - 2\lambda_2 \cos \omega) + d_{11, 2}(1 - \lambda_2^2)(1 + \lambda_1^2 - 2\lambda_1 \cos \omega)}{(1 + \lambda_1^2 - 2\lambda_1 \cos \omega)(1 + \lambda_2^2 - 2\lambda_2 \cos \omega)}.
\end{aligned}
$$ (eq-54)

Note that the numerator of the last expression is not a function of $\cos \omega$, as a consequence of {eq}`eq-53`.[^fn16] To find a maximum of {eq}`eq-54`, we need only to find a minimum of the denominator. The first derivative of the denominator is

[^fn16]: The numerator is always nonnegative since the spectral density in general is nonnegative, as the quadratic form $b_m D_g \Gamma_0^* b_m'$ in {eq}`eq-44` can be shown to be positive semidefinite, by writing $\frac{1}{2}(D_g \Gamma_0^* + \Gamma_0^* D_g) = D_p W D_p + D_q W D_q$ where the diagonal matrices $D_p$ and $D_q$ consist respectively of $p_i = \frac{1 - \lambda_i \cos \omega}{1 + \lambda_i^2 - 2\lambda_i \cos \omega}$ and $q_i = \frac{\lambda_i \sin \omega}{1 + \lambda_i^2 - 2\lambda_i \cos \omega}$ and where $W$ is positive semidefinite.

$$
2[(1 + \lambda_1^2)\lambda_2 + (1 + \lambda_2^2)\lambda_1] \sin \omega - 8\lambda_1 \lambda_2 \cos \omega \sin \omega.
$$ (eq-55)

For $0 < \omega < \pi$, $\sin \omega$ is positive. Hence, the derivative {eq}`eq-55` will be zero if and only if

$$
(1 + \lambda_1^2)\lambda_2 + (1 + \lambda_2^2)\lambda_1 - 4\lambda_1 \lambda_2 \cos \omega = 0.
$$ (eq-56)

When {eq}`eq-56` holds, the second derivative of the denominator is

$$
2 \sin \omega \left[ (1 + \lambda_1^2)\lambda_2 + (1 + \lambda_2^2)\lambda_1 + 4\lambda_1 \lambda_2 \sin \omega \right].
$$ (eq-57)

Let $\lambda_1$ and $\lambda_2$ be conjugate complex, as given by {eq}`eq-28`. Substitution into {eq}`eq-56` gives

$$
2r(1 + r^2)\cos \theta - 4r^2 \cos \omega = 0 \quad \text{or} \quad \cos \omega = \frac{1 + r^2}{2r} \cos \theta.
$$ (eq-58)

When {eq}`eq-58` holds, the second derivative {eq}`eq-57` will be positive if and only if $(\cos \omega + \sin \omega)$ is positive, i.e., $\omega < \frac{3}{4}\pi$, guaranteeing a maximum in the spectral density. Since $-1 < \cos \omega < 1$, the necessary condition {eq}`eq-58` for a maximum in the spectral density is

$$
-1 < \frac{1 + r^2}{2r} \cos \theta < 1.
$$ (eq-59)

If the absolute value $r$ of the roots is close to one, so that the factor $(1 + r^2)/2r$ is also close to one, the condition {eq}`eq-59` will be satisfied; in fact, by {eq}`eq-58` the frequency $\omega$ that corresponds to a peak in the spectral density will be close to the frequency $\theta$ of the roots. On the other hand, if $r$ is small, so that $(1 + r^2)/2r$ is large, the condition {eq}`eq-59` can be met only if $\cos \theta$ is close to zero, or the frequency $\theta$ is close to $\pi/2$, which corresponds to cycles of approximately 4 periods. For example, if $\theta = 54°$, corresponding to cycles of approximately 6.67 periods, $\cos \theta$ is .5878. An absolute value $r$ of .3 will give a factor of 1.817, violating the necessary condition {eq}`eq-59`. An absolute value of .4 will give $\cos \omega = 1.450(.5878) = .8523$, or $\omega = 31.5°$, corresponding to cycles of 11.4 periods, much longer than the 6.67-period cycle of the deterministic model.

If the roots are real and positive in the second-order equation, the necessary condition {eq}`eq-56` cannot be satisfied, since

$$
\cos \omega = \frac{(1 + \lambda_1^2)\lambda_2 + (1 + \lambda_2^2)\lambda_1}{4\lambda_1 \lambda_2} > 1
$$ (eq-60)

or

```{math}
:enumerated: false
(1 + \lambda_1^2)\lambda_2 + (1 + \lambda_2^2)\lambda_1 - 4\lambda_1 \lambda_2 > 0.
```

The last inequality is equivalent to

$$
\lambda_1 (1 - \lambda_2)^2 + \lambda_2 (1 - \lambda_1)^2 > 0
$$ (eq-61)

which certainly holds under our assumption.

While real and positive roots alone in the second-order equation {eq}`eq-48` cannot generate distinct cycles in the spectral sense, it is important to emphasize that they can indeed do so in the general linear model {eq}`eq-13`, even when the matrix $A$ is of dimension two. To demonstrate this point, let us examine the derivative of {eq}`eq-44`, which is a linear combination of the derivatives of $g_i$

$$
\frac{dg_i}{d\omega} = \frac{-(2 \sin \omega)\lambda_i (1 - \lambda_i^2)}{(1 + \lambda_i^2 - 2\lambda_i \cos \omega)^2} = -(2 \sin \omega) h_i
$$ (eq-62)

with $h_i$ defined as

$$
h_i = \frac{\lambda_i (1 - \lambda_i^2)}{(1 + \lambda_i^2 - 2\lambda_i \cos \omega)^2} \qquad (i = 1, \ldots, p).
$$ (eq-63)

From {eq}`eq-44` and {eq}`eq-62`, denoting by $D_h$ the diagonal matrix consisting of $h_i$,

$$
\frac{df_{mm}(\omega)}{d\omega} = (-2 \sin \omega) b_m D_h \Gamma_0^* b_m'.
$$ (eq-64)

As $\sin \omega$ is positive for the relevant range $0 < \omega < \pi$, the derivative {eq}`eq-64` is opposite in sign to the quadratic form

$$
b_m D_h \Gamma_0^* b_m'.
$$ (eq-65)

If this quadratic form is definite, the spectral density will have no maximum for $0 < \omega < \pi$. Otherwise, we can choose a vector $b_m$ to make the form {eq}`eq-65` vanish. The choice of $B$ is independent of the choice of $W = B^{-1} V B'^{-1}$ since $V$ can always be specified as $B W B'$.

The fact that all roots are real and positive does not guarantee the form {eq}`eq-65` to be positive definite. As an example, let

$$
\lambda_1 = .1, \quad w_{11} = w_{22} = 1, \quad b_{m1} = 1, \quad w_{12} = .8, \quad b_{m2} = -.01.
$$ (eq-66)

The form {eq}`eq-65` will not be positive definite, and the spectral density will be, by {eq}`eq-44`,

$$
b_m D_g \left( \frac{w_{ij}}{1 - \lambda_i \lambda_j} \right) b_m' = \frac{.9913}{1.01 - .2 \cos \omega} - \frac{.001570}{1.81 - 1.8 \cos \omega}.
$$ (eq-67)

Selected values of the density {eq}`eq-67` are:

```{list-table} Selected values of the spectral density $f_{mm}(\omega)$
:header-rows: 1
:name: tbl-spectral-density

* - $\omega$
  - $0$
  - $\frac{\pi}{16}$
  - $\frac{\pi}{8}$
  - $\frac{2\pi}{8}$
  - $\frac{3\pi}{8}$
  - $\frac{4\pi}{8}$
  - $\frac{5\pi}{8}$
  - $\frac{6\pi}{8}$
  - $\frac{7\pi}{8}$
  - $\pi$
* - $f_{mm}(\omega)$
  - 1.067
  - 1.183
  - 1.191
  - 1.138
  - 1.061
  - .981
  - .912
  - .860
  - .829
  - .819
```

The peak (at $\omega$ slightly below $.1\pi$) is quite pronounced.

This example reminds us of the well-known result of Slutsky[^fn17] that taking certain moving averages of a random series can generate cycles. Our model

[^fn17]: See, for example, M. G. Kendall and A. Stuart, *The Advanced Theory of Statistics* (London: Charles Griffin, 1966), Vol. 3, pp. 378 and 414–15. {cite}`kendall1966`

$$
y_t = u_t + A u_{t-1} + A^2 u_{t-2} + \cdots
$$ (eq-68)

amounts to taking an infinite moving average of the random vectors $u_t$ with "geometrically declining" weights, $A^0, A^1, A^2, \ldots$, in matrix terms. Although there can be no distinct cycles if $A$ is a scalar between zero and one, the situation is different for a matrix $A$ with roots between zero and one. To put it differently, when neither of two (canonical) variables

```{math}
:enumerated: false
z_{1t} = \lambda_1 z_{1, t-1} + \epsilon_{1t}, \quad z_{2t} = \lambda_2 z_{2, t-1} + \epsilon_{2t}
```

has distinct cycles (with $\lambda_1 = .1$ and $\lambda_2 = .9$, say), a linear combination, say $z_{1t} - .01 z_{2t}$, can have a peak in its spectral density.

(sec-conclusions)=
## VI. Conclusions

Before concluding, I would like to comment briefly on the case when a root, say $\lambda_1$, is greater than one. For this case, {cite}`quenouille1957` has claimed that (A) any univariate time series

```{math}
:enumerated: false
y_t = \lambda_1 y_{t-1} + \epsilon_t \qquad (\lambda_1 > 1)
```

can be decomposed into an exponential trend plus a stationary first-order series, that (B) the trend and the stationary series are respectively $x_t = \lambda_1 x_{t-1}$ and

```{math}
:enumerated: false
y_t^* = \lambda_1^{-1} y_{t-1}^* + \eta_t
```

and that (C), in general, any nonstationary autoregressive process with real roots may be partitioned in a similar manner, where the remaining stationary scheme is determined by his discussion on identification. If assertions (A) and (B), or even (A) alone, are accepted, the trend in a nonstationary canonical variable can be eliminated, and the resulting system can be treated as stationary even if some roots are complex. This subject is discussed in another paper.[^fn18]

[^fn18]: G. C. Chow and R. E. Levitan, "Spectral Properties of Non-stationary Systems of Linear Stochastic Difference Equations," IBM Research Report, RC-2059, April 1968. {cite}`chow_levitan1968a`

This paper has begun with a formulation of the acceleration principle. In a deterministic model consisting only of demand equations which obey simple distributed lags, the acceleration equation is necessary for prolonged oscillations. However, when random shocks are introduced, prolonged oscillations in the deterministic system (complex roots) will be neither necessary nor sufficient for generating distinct cycles — although, in the Hansen–Samuelson multiplier-accelerator model, complex roots are necessary, and, if their absolute value is large, sufficient. An obvious moral is that the nature of business cycles can be understood only by an integrated view of the deterministic as well as the random elements.

As far as the spectral densities of economic time series are concerned, {cite}`granger1966` has reported on a "typical spectral shape," i.e., $f(\omega)$ as a monotone decreasing function of $\omega$, and has suggested a set of first-order autoregressive equations, e.g.,

```{math}
:enumerated: false
y_t = a y_{t-1} + \epsilon_t
```

to explain this shape. In view of the possibilities that economic models may contain complex roots, and that, even with only real and positive roots, they may generate distinct cycles, is one willing to accept this shape as a good approximation? Only more empirical work will tell. But the approach to ascertaining the spectral shape is perhaps not to do more spectral analysis (which applies little or no restriction on the density), but to analyze the spectral densities implicit in econometric models.[^fn19]

[^fn19]: See G. C. Chow and R. E. Levitan, "Nature of Business Cycles Implicit in a Linear Economic Model," IBM Research Report, RC-2085, May 1968, which also deals with cross-spectral densities. {cite}`chow_levitan1968b`
