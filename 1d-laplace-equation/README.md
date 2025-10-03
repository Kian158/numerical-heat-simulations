# 2D Laplace Equation Solver (Jacobi Method)

A numerical simulation in Python that solves the **2D Laplace equation** using the **finite difference method** and the **Jacobi iterative solver**. The result is a steady-state potential field over a 2D square grid.

---

## Problem Overview

This script solves the **Laplace equation** in two dimensions:

> ∇²φ(x, y) = 0

Under fixed boundary conditions. The solution represents the **steady-state potential field** in a region with specified boundary voltages.

---

## Method

I discretized the 2D domain into an (N+1) × (N+1) grid and apply the **Jacobi iterative method** using the finite difference approximation:

φ[i, j] = 0.25 * (φ[i+1, j] + φ[i-1, j] + φ[i, j+1] + φ[i, j-1])

Boundary conditions are applied at the **top and bottom edges**, fixed at `V = 1`, while the left and right sides are held at 0 V by default.

<img width="501" height="418" alt="6 1 graph" src="https://github.com/user-attachments/assets/bac5d74b-2d51-429f-a01b-5d1f93e2739a" />
