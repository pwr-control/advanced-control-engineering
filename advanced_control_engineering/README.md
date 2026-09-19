# Advanced Control Engineering — lecture notes

`advanced_control_engineering.tex` (October 2022, updated since), compiled to
`advanced_control_engineering.pdf`. A self-contained treatment from state-space
representation to nonlinear and optimal control, with examples drawn from power electronics,
electrical drives and mechatronics.

## Contents

1. **Linear System Theory and Design** — state-space representation, discretization,
   canonical forms, controllability, state feedback, observability, duality, state observer,
   state feedback with integrator.
2. **Ljapunov Stability** — background, fundamentals, first and second criterion, analysis of
   LTI systems.
3. **Optimal Control** — general continuous-time problem, LQR, steady-state LQ, optimal
   control of the mass-spring-mass system, LQI control.
4. **Least Squares Parameters Estimation for Dynamical Systems** — non-recursive and
   recursive least squares.
5. **The Kalman Theory** — linear least-squares problem, the Kalman-filter problem.
6. **Model Predictive Control** — predictive current control of a single-phase RL load,
   theory of MPC.
7. **Adaptive Control** — model reference adaptive control, simple adaptive systems,
   adaptive control of an active suspension.
8. **Dynamical System Models Derivation** — permanent-magnet linear actuator (moving coil),
   PMSM, induction motor, lithium-ion battery, LRCL circuit, generic thermal model.
9. **Control System Design: case studies** — control of a wheel with C-code implementation
   (C-Caller), mass-spring-mass, single-phase inverter, moving coil, pendulum on cart,
   segway, lithium-ion battery management with EKF, PMSM MPC with EKF, induction motor
   control with Kalman observer, control of a harmonic in harsh environment, magnetic
   bearing modelling and control.
10. **Appendices** — moving reference frames, propaedeutic fundamentals for magnetic bearings.

## Figures

`figures/` is organized by topic/case study (`adaptive_control`, `ccaller`, `discretization`,
`double_integrator`, `generic_thermal_model`, `kalman`, `least_square`,
`lithium_ion_battery`, `ljapunov`, `lrcl_circuit`, `magnetic_bearing`, `moving_coil`, `mpc`,
`msm`, `optimal_control`, `pendulum_on_cart`, `pi_discrete`, `pmsm`, `segway`, `shaker`,
`single_phase_inverter`, `state_fb`, `vector_modulator`, `appendix`). Simulation figures are
the EPS files printed by the plotting scripts of the corresponding projects in
`lectures-on-advanced-control-engineering`.
