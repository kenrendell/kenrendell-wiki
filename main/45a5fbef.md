---
date: 2023-08-21
tags:
  - ac
  - circuit
  - phasor
  - impedance
  - admittance
  - resistance
  - conductance
  - reactance
  - susceptance
---

# Impedance and Admittance

From the [phasor voltage-current relations of circuit elements](867477c8.md).

| Element | Impedance | Admittance |
| :-: | :-: | :-: |
| [Resistor](427b2567.md) $R$ | $\displaystyle \mathbf{Z} = R$ | $\displaystyle \mathbf{Y} = \frac{1}{R}$ |
| [Inductor](8be49ac8.md) $L$ | $\displaystyle \mathbf{Z} = j\omega L$ | $\displaystyle \mathbf{Y} = \frac{1}{j\omega L}$ |
| [Capacitor](48507115.md) $C$ | $\displaystyle \mathbf{Z} = \frac{1}{j\omega C}$ | $\displaystyle \mathbf{Y} = j\omega C$ |

## Impedance

> The ***impedance*** $\mathbf{Z}$ of a circuit is the ratio of the [phasor](82b1dcbd.md) voltage $\mathbf{V}$ to the [phasor](82b1dcbd.md) current $\mathbf{I}$, measured in ohms $\mathit{\Omega}$.
>
> $\boxed{\mathbf{Z} = \frac{\mathbf{V}}{\mathbf{I}}}$

The impedance represents the opposition that the circuit exhibits to the flow of sinusoidal current. Although the impedance is the ratio of two [phasors](82b1dcbd.md), it is not a phasor, because it does not correspond to a sinusoidally varying quantity.

From the table, $\mathbf{Z}_L = j\omega L$ and $\mathbf{Z}_C = 1/\left(j\omega C\right)$. When angular frequency $\omega = 0$ (for dc sources), $\mathbf{Z}_L = 0$ (short circuit) and $\mathbf{Z}_C \rightarrow \infty$ (open circuit). When $\omega \rightarrow \infty$ (for high frequencies), $\mathbf{Z}_L \rightarrow \infty$ (open circuit) and $\mathbf{Z}_C = 0$ (short circuit).

As a complex quantity, the *impedance* may be expressed in rectangular form and polar form.

> $\boxed{\mathbf{Z} = R + jX = \left|\mathbf{Z}\right|\angle\theta}$
>
> where
>
> $\displaystyle \left|\mathbf{Z}\right| = \sqrt{R^2 + X^2}$
>
> $\displaystyle \theta = \tan^{-1}\left(\frac{X}{R}\right)$
>
> $\displaystyle R = \left|\mathbf{Z}\right|\cos\left(\theta\right)$
>
> $\displaystyle X = \left|\mathbf{Z}\right|\sin\left(\theta\right)$

where $R = \textrm{Re}\left(\mathbf{Z}\right)$ is the *resistance* and $X = \textrm{Im}\left(\mathbf{Z}\right)$ is the ***reactance***. The impedance is ***inductive*** when $X$ is positive or ***capacitive*** when $X$ is negative. Thus, impedance $\mathbf{Z} = R + jX$ is said to be *inductive* or lagging since current lags voltage, while impedance $\mathbf{Z} = R - jX$ is *capacitive* or leading bacause current leads voltage. The *impedance*, *resistance*, and *reactance* are all measured in ohms $\mathit{\Omega}$.

> For *capacitive reactance* $X_C$
>
> $\boxed{X_C = \frac{1}{\omega C}}$
>
> For *inductive reactance* $X_L$
>
> $\boxed{X_L = \omega L}$

## Admittance

> The ***admittance*** $\mathbf{Y}$ is the reciprocal of impedance $\mathbf{Z}$, measured in siemens (S).
>
> $\boxed{\mathbf{Y} = \frac{1}{\mathbf{Z}} = \frac{\mathbf{I}}{\mathbf{V}}}$

As a complex quantity, the *impedance* may be expressed in rectangular form.

> $\boxed{\mathbf{Y} = G + jB}$

where $G = \textrm{Re}\left(\mathbf{Y}\right)$ is the *conductance* and $B = \textrm{Im}\left(\mathbf{Y}\right)$ is the ***susceptance***. The *admittance*, *conductance*, and *susceptance* are all expressed in the unit of siemens (or mhos).

Showing that conductance $G \ne 1/R$ as it is in resistive circuits.

> $\displaystyle G + jB = \frac{1}{R + jX}$
>
> By rationalization
>
> $\displaystyle G + jB = \frac{1}{R + jX}\cdot\frac{R - jX}{R - jX} = \frac{R - jX}{R^2 + X^2}$
>
> Equating the real and imaginary parts gives
>
> $\displaystyle G = \frac{R}{R^2 + X^2}$
>
> $\displaystyle B = -\frac{X}{R^2 + X^2}$
