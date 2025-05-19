# Improved PINN for Heat Equation

This implementation provides an enhanced Physics-Informed Neural Network (PINN) model for solving the 1D heat equation. The improvements address issues with the original implementation to achieve better accuracy and convergence between the PINN prediction and the exact solution.

## Problem Description

The 1D heat equation with boundary and initial conditions:

```
∂u/∂t = ∂²u/∂x² for x ∈ [0, 1], t > 0
```

**Initial Condition:** u(x, 0) = sin(πx)

**Boundary Conditions:** u(0, t) = 0, u(1, t) = 0 for all t ≥ 0

**Analytical Solution:** u(x, t) = sin(πx) · e^(-π²t)
