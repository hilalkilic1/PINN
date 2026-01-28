# Physics-Informed Neural Networks (PINNs) for Black Hole Dynamics

A deep learning framework designed to investigate the **vacuum field equations** of spherically symmetric black holes in the near-horizon regime. This project leverages **Physics-Informed Neural Networks (PINNs)** to solve the Einstein Field Equations (EFE) by embedding gravitational constraints directly into the network's loss function.



## Problem Statement
The investigation of spacetime curvature near a Schwarzschild black hole requires solving non-linear partial differential equations. This project explores the **near-horizon dynamics** where standard numerical relativity can face coordinate singularities. The model approximates the metric components $g_{\mu\nu}$ while enforcing the vacuum condition:
$$G_{\mu\nu} = 0$$

## Methodology
* **Physics-Informed Loss:** The loss function incorporates the **Residual of the Einstein Field Equations**, penalizing deviations from physical spacetime solutions.
* **Gravitational Constraints:** Leverages PINNs to satisfy fundamental gravitational constraints specifically within the high-gravity, near-horizon regime.
* **Symmetry Exploitation:** By assuming spherical symmetry, the problem is reduced to finding the radial and temporal components of the metric, optimizing the network’s search space.



## Technical Stack
* **Framework:** PyTorch
* **Domain:** General Relativity, Differential Geometry, Automatic Differentiation (Autograd).
* **Research Focus:** Vacuum solutions and horizon-scale dynamics.

## Key Results
* Demonstrated that PINNs can satisfy the **Hamiltonian Constraint** in vacuum to within a high degree of precision.
* Reproduced expected metric behavior for static, spherically symmetric configurations without the use of traditional mesh-based numerical solvers.
