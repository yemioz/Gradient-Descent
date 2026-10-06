# Gradient-Descent

A from-scratch implementation of the gradient descent algorithm in Python, built to demonstrate how the method converges to a function's minimum step by step.

## Overview

Gradient descent is an iterative optimization algorithm that moves toward a function's minimum by repeatedly stepping in the direction of steepest descent:
$$x_{n+1} = x_n - \alpha f(x_n)


This notebook implements that update rule using symbolic differentiation rather than a hardcoded derivative, so the method generalizes beyond the specific test function.

## Approach

- Used SymPy to symbolically differentiate the objective function, then converted the derivative to a callable function with `lambdify`
- Tested on f(x) = x², which has a known minimum at x = 0, to validate convergence
- Ran 50 iterations from an initial guess of x₀ = 4 with learning rate α = 0.2
- Tracked and plotted each iteration's solution against the function curve to visualize convergence

## Result

The algorithm converges to the known minimum (x = 0) within the 50 iterations, confirming the implementation behaves as expected before applying it to problems without a known closed-form answer.

## Tools

Python, NumPy, SymPy, Pandas, Matplotlib, SciPy

## Background

Built to support a 30-minute technical presentation on gradient descent delivered to technical and non-technical faculty and staff, walking through the algorithm from theory to a working implementation.
