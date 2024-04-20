---
date: 2023-10-06
tags:
  - status/ongoing
  - system
  - signal
---

# Digital Filters

A digital filter may be described by the [difference equation](72022de7.md)

> $\boxed{y[n] + A_{1}\,y[n - 1] + \cdots + A_{N}\,y[n - N] = B_{0}\,x[n] + B_{1}\,x[n - 1] + \cdots + B_{M}\,x[n - M]}$

##  Digital Filter Realization

Digital filters described by difference equations can be realized by using the symbolic elements: **gain** (scalar multiplier), **delay** (shift), and **summer** (or **adder**).
