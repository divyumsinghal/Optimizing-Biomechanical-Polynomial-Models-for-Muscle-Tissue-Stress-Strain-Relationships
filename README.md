# Optimizing Biomechanical Polynomial Models for Muscle Tissue Stress-Strain Relationships

## Overview

This repository contains MATLAB code for optimizing biomechanical polynomial models to characterize the stress-strain relationships in human muscle tissue. The focus is on the transverse (cross-fiber XF) direction, and the code explores different polynomial orders and fitting methods to achieve an accurate model.

## Contents

1. **Code File:** [`Optimizing_Biomechanical_Polynomial_Models.mlx`](Optimizing_Biomechanical_Polynomial_Models.mlx)
   - MATLAB Live Script containing the code for the optimization process.

2. **Data File:** [`muscle_data_2023.xlsx`](muscle_data_2023.xlsx)
   - Excel file containing stress-strain data for muscle tissue.

## Project

Understanding the compressive properties of human muscle tissue is crucial for various fields, including impact biomechanics, surgical simulation, and rehabilitation engineering. This MATLAB project focuses on optimizing biomechanical polynomial models to accurately represent the stress-strain relationships in muscle tissue, particularly in the transverse (cross-fiber XF) direction.

The primary loading direction, transverse to the muscle fiber direction, is explored through compression tests on muscle samples. Tests conducted at TCD on pig muscle samples using a universal testing machine revealed nonlinear anisotropic behavior under quasi-static loading conditions. The challenge arises from the non-linearity of the stress-strain relationship, making it essential to move beyond simplistic linear models.

The project unfolds in several tasks:

1. **Visualization of Stress-Strain Data:**
   - Plotting the observed stress against strain to visualize the raw data.

2. **Polynomial Model Fitting:**
   - Employing polynomial regression with least-squares fitting to find the optimal model order.
   - Calculating the sum squared error for various model orders and selecting the best-fit polynomial model.

3. **Estimation and Visualization:**
   - Estimating the stress values using the selected polynomial model order and superimposing the result on the original plot.
   - Assessing the model fit through error calculation and visualization.

4. **Robust Model Fitting:**
   - Introducing a robust approach by minimizing the sum of absolute differences for a fourth-order polynomial model.
   - Superimposing the robust model on the original plot for comparison.

5. **Model Evaluation:**
   - Calculating the Mean Squared Error (MSE) for both the robust and least-squares fits in a defined sample range.
   - Demonstrating the potential advantages of the robust model in an area not corrupted by outliers.

This project aims to showcase the importance of advanced modeling techniques in accurately representing the biomechanical behavior of muscle tissue. The optimization process seeks to improve model performance, providing valuable insights for applications in impact biomechanics, surgical simulation, and rehabilitation engineering. The methodologies employed demonstrate a comprehensive approach to understanding and optimizing the stress-strain relationships in muscle tissue, contributing to advancements in biomechanics and related fields.

## Tasks

### Task 1: Plot Observed Stress vs. Strain
- Visualizes the original stress-strain data.

### Task 2: Fit Data to Polynomial Models
- Explores polynomial models of different orders using least-squares (LS) fitting.
- Identifies the optimal model order.

### Task 3: Plot Estimated Signal
- Calculates and superimposes the estimated stress based on the selected model order.

### Task 4: Calculate Error and Coefficient of Determination
- Computes errors and assesses the model fit through a histogram and coefficient of determination (R-squared).

### Task 5: Fit Stress Data to Polynomial of Order 4 with Absolute Error
- Applies absolute error minimization to fit stress data to a fourth-order polynomial.

### Task 6: Calculate Mean Squared Error (MSE)
- Measures MSE for both robust (absolute error minimization) and LS fitting in a specified sample range.

## License

This code is provided under the [GPL-3.0 license](LICENSE).