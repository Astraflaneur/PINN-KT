# PINN-KT: Finite Volume Methods for Physics-Informed Neural Networks

**Overview**:
PINN-KT is a research repository focused on the intersection of classical numerical methods and deep learning for solving computational physics problems. The core idea is to leverage Finite Volume Methods (FVM) within Physics-Informed Neural Networks (PINNs), enabling the neural network to learn solutions to partial differential equations (PDEs) using numerical discretization schemes rather than relying solely on automatic differentiation.

This approach, called FV-PINNs, integrates the physics of the underlying numerical method (e.g., flux gradients, RK time integration) directly into the training process, providing a robust framework for data-driven and physics-constrained modeling.


<img src=./figures/Sod.gif width="350" height="350"/><img src=./figures/L_u_PINNs_2033.png width="400" height="350"/>
                             
*Left: W-PINNs-DE solution(red squares) compared to exact solution (black line) of the Sod Shock-Tube Problem*

*Right: W-PINNs solution of deformation in x direction on Domain II*

<img src=./figures/BLP-OF.gif width="350" height="350"/><img src=./figures/Buckley-Leverett-Problem-full.png width="400" height="350"/>
                             
*Left: W-PINNs-DE solution (red squares) compared to exact solution (black line) of the Buckley-Leverett Problem*

*Right: Full W-PINNs-DE solution of Buckley-Leverett Problem*

## Features

- 1D & 2D Compressible Euler Equations: Forward and inverse shock-tube problems using PINNs and FVM.
- Burgers' Equation: Classic nonlinear PDE solved with PINNs.
- Linear Elasticity: Plane stress boundary value problems with domain extension.
- Visualization: High-quality figures and animations for solution comparison and analysis.
- Experimentation: Notebooks and scripts for rapid prototyping and benchmarking.

## Directory Structure

- burgers.equation/ — PINN implementations for Burgers' equation (forward/inverse).
- compressible.flow/ — Euler equations for compressible flow (1D/2D, forward/inverse).
- linear.elasticity/ — Plane stress elasticity problems and domain data.
- notebooks/ — Jupyter notebooks for interactive experiments.
- figures/ — Solution plots and animations.
- presentation_material/ — Reports and presentations summarizing results.

## Getting Started

1. **Install Dependencies**: See requirements.txt or use the provided setup scripts.
2. **Run Experiments**: Use the notebooks or Python scripts in each subfolder.
3. **Visualize Results**: Output files and figures are generated for analysis.

## Reference
Original work by Alexandros Papados.
Based on the paper:
Physics-Informed Deep Learning and its Application in Computational Solid and Fluid Mechanics (Papados, 2021)

