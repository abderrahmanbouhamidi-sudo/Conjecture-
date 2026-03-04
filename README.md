# Discrete Dynamical Systems modulo $2^p + 2^q$

Official repository for the **Bouhamidi Conjecture** (ArXiv:2601.06208).

## 📜 Overview / Présentation
This project explores the convergence properties of iterative maps $T_{p,q}$ defined on positive integers. This study extends the framework of the **Collatz conjecture**.

Ce projet explore les propriétés de convergence des applications itératives $T_{p,q}$ définies sur les entiers positifs. Cette étude généralise le cadre de la **conjecture de Collatz**.

### The Map / L'application $T_{p,q}$
For $p \ge q \ge 0$:

$$T_{p,q}(n)=\begin{cases} 
\frac{n}{d} & \text{if } n \equiv 0 \pmod{d} \\ 
\frac{\alpha n + \beta [n]_{d}}{d} & \text{if } n \not\equiv 0 \pmod{d} 
\end{cases}$$

Where $d = 2^p + 2^q$, $\alpha = 2^p + 2^{q+1}$,  $\beta = 2^p$ and $[n]_d$ stands for the reast in The Euclidean division of $d$ by $n$.

## 🚀 Interactive Simulator
The simulator allows users to visualize trajectories and identify cycles.

👉 **[Launch the Simulator / Lancer le simulateur](index.html)**

## 📚 Reference / Référence
If you use this work or the simulator, please cite the original paper:
Si vous utilisez ce travail, merci de citer l'article original :

> **Bouhamidi, S.** (2026). *Discrete Dynamical Systems modulo $2^p+2^q$*. [arXiv:2601.06208](https://doi.org/10.48550/arXiv.2601.06208)

---
© 2026 - Licensed under CC BY-NC-ND 4.0
