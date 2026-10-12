# Week 05 - Double Pendulum Chaos Simulation

## Experiment Information

| Item | Details |
|------|---------|
| Course | NCU Bioengineering Lab Course |
| Week | 05 |
| Experiment | Double Pendulum Chaos Simulation |
| Experimenter | Xu Ying |
| Student ID | 7904126062 |
| Major | Bioengineering, Nanchang University |

## Overview

A double pendulum simulator demonstrating chaotic dynamics through real-time numerical simulation. The system is solved using 4th-order Runge-Kutta (RK4) integration of the Lagrangian equations of motion.

## Features

- **RK4 Integration**: High-precision 4th-order Runge-Kutta solver at 240Hz physics step
- **Chaotic Dynamics**: Full Lagrangian mechanics for coupled nonlinear oscillation
- **Rainbow Trail**: HSL color-cycling trail with quadratic alpha fade on the second bob
- **Interactive Drag**: Mouse/touch drag either pendulum bob to set initial angles
- **Real-time HUD**: Displays angles, angular velocities, total energy, and simulation time
- **Adjustable Parameters**: Two pendulum lengths, mass ratio, gravity, trail length

## How to Run

Open `index.html` in any modern browser. No build tools or dependencies required.

## Controls

| Control | Description |
|---------|-------------|
| L1 / L2 sliders | Adjust pendulum arm lengths |
| m2 slider | Adjust mass of second bob |
| g slider | Adjust gravitational acceleration |
| Trail slider | Adjust trail buffer length |
| Mouse drag | Drag either bob to set initial angle |
| Reset button | Restore default parameters and state |

## Physics

The double pendulum equations are derived from the Lagrangian:

L = T - V, where T is kinetic energy and V is potential energy of the two-mass system.

The resulting coupled ODEs are solved at each timestep using the classical RK4 method with dt = 1/240 s, ensuring energy conservation and numerical stability even during chaotic tumbling.

## Directory Structure

```
week05_pendulum_sim/
├── README.md    # This file
└── index.html   # Complete simulator (HTML + CSS + JS, single file)
```
