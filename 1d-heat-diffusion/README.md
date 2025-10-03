## 1D Heat Diffusion Simulator

A simple Python simulation of **1D heat conduction** using the finite difference method. A 1D rod is modelled with fixed boundary conditions.

## Physics Background

This simulation solves the **1D heat equation**:

> dT/dt = D * d²T/dx²

Where:
- `T(x, t)` is the temperature at position `x` and time `t`
- `D` is the thermal diffusivity of the material

We use an **explicit finite difference method (FTCS)**:
T[i] = T[i] + (D * dt / dx²) * (T[i+1] + T[i-1] - 2*T[i])

## Output

At the end of the simulation, the final temperature profile is plotted across the rod.

<img width="567" height="453" alt="1d heat graph" src="https://github.com/user-attachments/assets/a554da81-c956-415e-aae4-7c6c4b91a566" />
