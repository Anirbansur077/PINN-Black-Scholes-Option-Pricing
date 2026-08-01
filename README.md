# Physics-Informed Neural Network for Black-Scholes Option Pricing

Physics-Informed Neural Network for Black-Scholes Option Pricing using PyTorch and Automatic Differentiation

## Overview

This project investigates the application of Physics-Informed Neural Networks (PINNs)
for solving the Black-Scholes Partial Differential Equation (PDE) for European Call
and Put option pricing.

The PINN is implemented using PyTorch and Automatic Differentiation and is evaluated
against the analytical Black-Scholes solution.

## Objectives

- Solve the Black-Scholes PDE using a Physics-Informed Neural Network.
- Predict European Call and Put option prices.
- Incorporate PDE, initial-condition, and boundary-condition constraints.
- Compare PINN predictions with analytical Black-Scholes solutions.
- Compute financial Greeks using Automatic Differentiation.

## Technologies Used

- Python
- PyTorch
- NumPy
- SciPy
- Matplotlib
- Physics-Informed Neural Networks (PINNs)
- Automatic Differentiation

## Methodology

The project follows the following workflow:

1. Define the Black-Scholes PDE.
2. Generate training points over the asset-price and time domain.
3. Define the PINN architecture.
4. Formulate PDE, initial-condition, and boundary-condition losses.
5. Train the neural network.
6. Compare PINN predictions with analytical Black-Scholes solutions.
7. Evaluate the model using MAE, RMSE, and Maximum Absolute Error.
8. Compute financial Greeks using Automatic Differentiation.

## Model Architecture

The neural network uses:

- Input: Asset Price (S) and Time (t)
- Hidden Layers: Fully Connected Neural Network
- Activation Function: SiLU
- Weight Initialization: Xavier Initialization
- Framework: PyTorch

## Model Evaluation

The PINN predictions are compared with the analytical Black-Scholes solution
using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Maximum Absolute Error

## Financial Greeks

The project computes the following financial Greeks:

- Delta
- Gamma
- Vega
- Theta

These are obtained using Automatic Differentiation.

## Results

### European Call Option

| Metric | Value |
|---|---:|
| MAE | 0.0097 |
| RMSE | 0.0157 |
| Maximum Absolute Error | 0.0376 |

### European Put Option

| Metric | Value |
|---|---:|
| MAE | 0.0301 |
| RMSE | 0.0485|
| Maximum Absolute Error | 0.1125 |

