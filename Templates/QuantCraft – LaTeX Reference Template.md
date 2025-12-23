---
title: "{{title}}"
domain: QuantCraft
type: Reference
topic: LaTeX / Math Notation
level: All
tags:
  - quantcraft
  - latex
  - math
  - reference
  - numerical-analysis
created: {{date}}
---

# QuantCraft — LaTeX Reference Sheet

> **Purpose:** Canonical LaTeX / MathJax notation for QuantCraft notes  
> **Rule #1:** Multi-character superscripts & subscripts always use `{}`

---

## 1️⃣ Numbers, Exponents & Precision

### Powers
$$
10^{16}, \quad x^{n}, \quad e^{i\pi}
$$

### Scientific notation
$$
1.23 \times 10^{6}
$$

### Floating-point notation
$$
\operatorname{fl}(x)
$$

### Absolute value
$$
|x| \quad \text{or} \quad \lvert x \rvert
$$

---

## 2️⃣ Algebra & Calculus

### Fractions
$$
\frac{a}{b}
$$

### Roots
$$
\sqrt{x}, \quad \sqrt[n]{x}
$$

### Limits
$$
\lim_{x \to 0} f(x)
$$

### Derivatives
$$
\frac{df}{dx}, \quad \frac{\partial f}{\partial x}
$$

### Higher-order derivatives
$$
\frac{d^2 f}{dx^2}, \quad \frac{\partial^2 f}{\partial x^2}
$$

### Integrals
$$
\int f(x)\,dx, \quad \int_a^b f(x)\,dx
$$

---

## 3️⃣ Linear Algebra (Quant-Critical)

### Vectors
$$
\mathbf{x}, \quad \boldsymbol{\beta}
$$

### Matrices
$$
\mathbf{A}, \quad \Sigma
$$

### Transpose
$$
\mathbf{x}^\top
$$

### Inverse
$$
\mathbf{A}^{-1}
$$

### Norms
$$
\|\mathbf{x}\|, \quad \|\mathbf{x}\|_2
$$

### Dot product
$$
\mathbf{x} \cdot \mathbf{y}
$$

### Identity matrix
$$
\mathbf{I}
$$

---

## 4️⃣ Probability & Statistics

### Probability
$$
\mathbb{P}(A)
$$

### Expectation
$$
\mathbb{E}[X], \quad \mathbb{E}[X \mid Y]
$$

### Variance
$$
\operatorname{Var}(X)
$$

### Covariance
$$
\operatorname{Cov}(X, Y)
$$

### Correlation
$$
\rho_{XY}
$$

---

## 5️⃣ Common Distributions

### Normal
$$
X \sim \mathcal{N}(\mu, \sigma^2)
$$

### Log-normal
$$
X \sim \operatorname{Lognormal}(\mu, \sigma^2)
$$

### Bernoulli
$$
X \sim \operatorname{Bernoulli}(p)
$$

### Binomial
$$
X \sim \operatorname{Binomial}(n, p)
$$

---

## 6️⃣ Time Series & Stochastic Processes

### Time index
$$
X_t, \quad X_{t+1}
$$

### Returns
$$
r_t = \frac{P_t - P_{t-1}}{P_{t-1}}
$$

### Log returns
$$
r_t = \ln\left(\frac{P_t}{P_{t-1}}\right)
$$

### AR(1)
$$
X_t = \phi X_{t-1} + \epsilon_t
$$

### Brownian motion
$$
W_t
$$

### Geometric Brownian Motion
$$
dS_t = \mu S_t\,dt + \sigma S_t\,dW_t
$$

---

## 7️⃣ Optimization

### Argmax / Argmin
$$
\arg\max_x f(x), \quad \arg\min_x f(x)
$$

### Constraints
$$
\text{s.t. } g(x) \le 0
$$

### Lagrangian
$$
\mathcal{L}(x, \lambda)
$$

---

## 8️⃣ Sets, Logic & Indicators

### Common sets
$$
\mathbb{R}, \mathbb{Z}, \mathbb{N}, \mathbb{Q}
$$

### Indicator function
$$
\mathbb{1}_{\{x > 0\}}
$$

### Logic
$$
\forall \quad \exists \quad \implies \quad \iff
$$

---

## 9️⃣ Summations & Products

### Summation
$$
\sum_{i=1}^n x_i
$$

### Infinite sum
$$
\sum_{i=0}^{\infty}
$$

### Product
$$
\prod_{i=1}^n x_i
$$

---

## 🔟 QuantCraft Notation Table

| Concept | Notation |
|------|--------|
Vector | `\mathbf{x}` |
Expectation | `\mathbb{E}` |
Probability | `\mathbb{P}` |
Covariance | `\operatorname{Cov}` |
Volatility | `\sigma` |
Noise | `\epsilon_t` |
Correlation | `\rho` |
Risk-free rate | `r_f` |

---

## 🧠 Notes / Extensions
- Add domain-specific notation here
- Keep this file as the **single source of truth**
- Link to it from all QuantCraft chapters

