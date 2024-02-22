# Computational Fluid Dynamics (CFD) Simulations

This repository contains a collection of Computational Fluid Dynamics simulations implemented in Python. These simulations are based on solving the Navier-Stokes equations for various fluid dynamics phenomena, including convection, diffusion, Burgers' equation, Laplace's equation, Poisson's equation, cavity flow, and channel flow. Each simulation demonstrates fundamental concepts in fluid mechanics and numerical methods.

## Features

- **Linear Convection**: Simulation of wave propagation in a fluid using the first-order linear convection equation.
- **Nonlinear Convection**: Demonstrates the propagation of waves with nonlinear effects.
- **Diffusion**: Models the diffusion process of a substance in a fluid.
- **Burgers' Equation**: A combination of nonlinear convection and diffusion, illustrating shock wave formation and diffusion.
- **Laplace's Equation**: Solves Laplace's equation to find potential fields in static fluid and electrostatics scenarios.
- **Poisson's Equation**: Similar to Laplace's equation but includes a source term to represent phenomena like electrostatic potential fields with charge distributions.
- **Cavity Flow**: Simulates fluid flow in a square cavity driven by the motion of one of the cavity walls.
- **Channel Flow**: Demonstrates fluid flow through a channel driven by a pressure gradient.

## Simulations Overview

### Linear and Nonlinear Convection

- **Equations**: 
  - Linear: \(\frac{\partial u}{\partial t} + c \frac{\partial u}{\partial x} = 0\)
  - Nonlinear: \(\frac{\partial u}{\partial t} + u \frac{\partial u}{\partial x} = 0\)

![Linear Convection](<Path-to-Linear-Convection-Image>)
![Nonlinear Convection](<Path-to-Nonlinear-Convection-Image>)

### Diffusion

- **Equation**: \(\frac{\partial u}{\partial t} = \nu \frac{\partial^2 u}{\partial x^2}\)

![Diffusion](<Path-to-Diffusion-Image>)

### Burgers' Equation

- **Equation**: \(\frac{\partial u}{\partial t} + u \frac{\partial u}{\partial x} = \nu \frac{\partial^2 u}{\partial x^2}\)

![Burgers' Equation](<Path-to-Burgers-Equation-Image>)

### Laplace's and Poisson's Equations

- **Laplace's Equation**: \(\nabla^2 \phi = 0\)
- **Poisson's Equation**: \(\nabla^2 \phi = f\)

![Laplace Equation](<Path-to-Laplace-Equation-Image>)
![Poisson Equation](<Path-to-Poisson-Equation-Image>)

### Cavity Flow

- **Navier-Stokes Equations for Incompressible Flow**:
  - Momentum equation (simplified for 2D): \(\frac{\partial u}{\partial t} + u \frac{\partial u}{\partial x} + v \frac{\partial u}{\partial y} = -\frac{1}{\rho}\frac{\partial p}{\partial x} + \nu \left(\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2}\right)\)
  - Continuity equation: \(\frac{\partial u}{\partial x} + \frac{\partial v}{\partial y} = 0\)

![Cavity Flow](<Path-to-Cavity-Flow-Image>)

### Channel Flow

- **Equations**: Similar to cavity flow, but with a pressure gradient driving the flow.

![Channel Flow](<Path-to-Channel-Flow-Image>)

## Dependencies

- numpy
- matplotlib
- scipy

## Usage

To run a simulation, use the following command:

```bash
python <simulation_script>.py
