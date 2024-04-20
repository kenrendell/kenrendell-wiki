---
date: 2023-08-23
tags:
  - singularity-function
  - signal
  - circuit
---

# Singularity Functions

Singularity functions (also called *switching functions*) are very useful in circuit analysis. They serve as good approximations to the switching signals that arise in circuits with switching operations.

> ***Singularity functions*** are functions that either are discontinuous or have discontinuous derivatives.

The three most widely used singularity functions in circuit analysis are the [unit step](58fcc503.md), the [unit impulse](b0a34c02.md), and the [unit ramp](9e65fb42.md) functions.

The three singularity functions are related by differentiation as

> $\displaystyle \delta\left(t\right) = \frac{d}{dt} u\left(t\right)$
>
> $\displaystyle u\left(t\right) = \frac{d}{dt} r\left(t\right)$
>
> or by integration as
>
> $\displaystyle r\left(t\right) = \int_{-\infty}^{t} u\left(\lambda\right)\,d\lambda$
>
> $\displaystyle u\left(t\right) = \int_{-\infty}^{t} \delta\left(\lambda\right)\,d\lambda$
