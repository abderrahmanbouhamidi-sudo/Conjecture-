# Discrete Dynamical Systems modulo $2^p + 2^q$

Official repository for the **Bouhamidi Dynamics** (ArXiv:2601.06208).  
This project explores the convergence properties and orbital structures of iterative maps $T_{p,q}$ defined on positive integers, extending the framework of the **Collatz conjecture**.

##  Mathematical Definition

For $p \ge q \ge 0$, the transition function $T_{p,q}(n)$ is defined as:

$$T_{p,q}(n)=\begin{cases} 
\frac{n}{d} & \text{if } n \equiv 0 \pmod{d} \\ 
\frac{\alpha n + \beta [n]_{d}}{d} & \text{if } n \not\equiv 0 \pmod{d} 
\end{cases}$$

Where:
- $d = 2^p + 2^q$ (The Divisor)
- $\alpha = 2^p + 2^{q+1}$ (The Multiplier)
- $\beta = 2^p$ (The Offset)
- $[n]_d$ denotes the remainder of the Euclidean division of $n$ by $d$ ($n \pmod d$).

---

##  Key Theoretical Results

### 1. The Trivial Cycle Theorem
We formally establish that for any pair $(p, q)$, a **trivial cycle** exists starting at $2^{p-q}$ with a deterministic length $L$:
$$L = 2^{p-q} + q + 1$$
This formula provides a predictable closed-form orbital structure for the entire family of maps, a feature typically absent in broader $ax+b$ generalizations.

### 2. Global Stability and Non-Divergence
The system is characterized by a strong contractive property. Let $\rho = \frac{\alpha}{d^2}$ be the characteristic growth ratio. For all $p, q \ge 0$:
$$\rho = \frac{2^p + 2^{q+1}}{(2^p + 2^q)^2} \le 0.75$$
Numerical analysis reveals an exponential decay of this ratio as $p$ scales:
- $\rho(0,0) = 0.75$ (Collatz equivalent)
- $\rho(14,14) \approx 4.58 \times 10^{-5}$
This negative drift ensures that trajectories are bounded, with no observed divergence to infinity across $10^8$ tested integers.

---

## Numerical Observations: The Exceptional Set $E$

While the trivial cycle is the global attractor for most parameters, we have identified a finite **Exceptional Set** $E$ where secondary cycles emerge. 

| Case $(p, q)$ | Trivial Basin (%) | Secondary Basin (%) | Secondary Cycle (Min. Element) |
| :--- | :---: | :---: | :--- |
| **(1, 0)** | 3.27% | 96.73% | 14 |
| **(2, 1)** | 96.22% | 3.78% | 74 |
| **(2, 2)** | 98.02% | 1.98% | 67 |
| **(3, 0)** | 94.26% | 5.74% | 280 |
| **(4, 0)** | 70.87% | 29.13% | 1264 |
| **(5, 2)** | 99.70% | 0.30% | 76200 / 87176 |
| **(6, 2)** | 79.32% | 20.68% | 1264 |
| **(7, 0)** | 99.79% | 0.21% | 3,027,584 |

---

##  Interactive Simulator & Theory
The repository includes an interactive web-based simulator (HTML5/JS) to visualize trajectories, calculate flight altitudes, and identify cycle elements in real-time.

 **[Launch the Simulator](index.html)**

For a detailed walkthrough of the mathematical proofs and the underlying logic:
 **[⬅ Back to the Theory](index.html)**

---

##  Reference & Citation
If you use this work, the simulator, or the datasets, please cite the original paper:

> **Bouhamidi, A. (2026). *Discrete Dynamical Systems modulo $2^p + 2^q$*. arXiv:2601.06208**

---
© 2026 - Licensed under CC BY-NC-ND 4.0

> **Bouhamidi, A.** (2026). *Discrete Dynamical Systems modulo $2^p+2^q$*. [arXiv:2601.06208](https://doi.org/10.48550/arXiv.2601.06208)

---
© 2026 - Licensed under CC BY-NC-ND 4.0
