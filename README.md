# Linear Regression for Auto Insurance in Sweden

## Description
This repository contains a Jupyter Notebook (`swdish_insurance_linear_regression.ipynb`) that demonstrates linear regression analysis on the Auto Insurance in Sweden dataset. The notebook explores the relationship between the number of claims and total payment for car insurance in Sweden.

## Dataset
The dataset used in this analysis is the "Auto Insurance in Sweden" dataset, which is available in the `insurance.txt` file within the repository. The real dataset was used to demonstrate simple linear regression. The dataset is called the “Auto Insurance in Sweden” dataset and involves predicting the total payment for all the claims in thousands of Swedish Kronor (y) given the total number of claims (x).

This means that for a new number of claims (x) we will be able to predict the total payment of claims (y).

## Requirements
To run the Jupyter Notebook and execute the code, you need the following dependencies:

- Python 3.x
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib

## Overview

This repository contains code for optimizing a linear regression model using the gradient descent algorithm. The primary goal of this code is to find the optimal weight (w) and bias (b) parameters that minimize the mean squared error (MSE) between the predicted values and actual values of a dataset.

## Code Components

### 1. `compute_cost` Function

The `compute_cost` function calculates the cost of the linear regression model given input data (`x`), actual output (`y`), weight (`w`), and bias (`b`). It uses the mean squared error (MSE) formula to measure the average squared difference between the predicted values and actual values.

### 2. `compute_gradient` Function

The `compute_gradient` function calculates the gradients of the cost function with respect to the weight (`w`) and bias (`b`). These gradients are essential for updating the model parameters during the gradient descent optimization process. The gradients are computed by taking the partial derivatives of the cost function.

### 3. `gradient_descent` Function

The `gradient_descent` function implements the gradient descent algorithm for optimizing the linear regression model. It takes several parameters, including input data (`x`), actual output (`y`), initial weights (`w_in`) and bias (`b_in`), cost and gradient calculation functions (`cost_function` and `gradient_function`), learning rate (`alpha`), and the number of iterations (`num_iters`).

During optimization, this function iteratively updates the weights and bias using the gradients computed by the `compute_gradient` function. It also stores the cost and weight history for analysis and prints the cost at regular intervals during training.

### 4. Initialization and Training

The code initializes the weight (`w`) and bias (`b`) to zero. It also specifies the number of iterations and the learning rate (`alpha`) for the gradient descent algorithm. These parameters should be chosen based on your specific problem and dataset.

## Usage

To use this code effectively, follow these steps:

1. Import the necessary libraries at the beginning of your script, such as `math` and `copy`.

2. Prepare your input data (`x_train`) and actual output (`y_train`) with your dataset.

3. Choose appropriate values for the learning rate (`alpha`) and the number of iterations (`num_iters`) based on your problem.

4. Call the `gradient_descent` function with your training data, parameters, and cost/gradient calculation functions to optimize the linear regression model.

5. After training, the code will print the learned values of `w` and `b` found by the gradient descent algorithm.

Note: There are additional parts of the code related to monitoring and debugging, such as saving the cost history and weight history. Additionally, there's a condition (`if i < 100000`) to prevent excessive resource consumption, which may not be necessary in all cases.

Feel free to modify and adapt this code to your specific requirements and datasets.
