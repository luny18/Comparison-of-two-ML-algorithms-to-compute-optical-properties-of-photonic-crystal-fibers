# Comparison-of-two-ML-algorithms-to-compute-optical-properties-of-photonic-crystal-fiber

This project explores the use of machine learning to predict key optical properties of photonic crystal fibers (PCFs), including the **effective index** and **effective mode area**

## Overview
Photonic crystal fibers (PCFs) are critical in various optical applications due to their unique properties. This study leverages two machine learning models, **LASSO** and **Random Forest**, to predict n_eff and A_eff based on PCF design parameters.

## Machine Learning Models
The following machine learning models were employed:
- **LASSO (Least Absolute Shrinkage and Selection Operator):** Effective for sparse feature selection and linear relationships.
- **Random Forest:** A robust ensemble learning method capable of capturing complex relationships.

## Dataset
The models were trained on a synthetic dataset of PCF parameters:
- **Wavelength:**
- **Pitch:**
- **Diameter-to-pitch ratio:** 
- **Number of air hole rings:**

## Performance Metrics
The performance of the models was evaluated using:
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **R-squared (\(R^2\))**

## Results
  - Random Forest outperformed LASSO with an \(R^2\) value of **0.99** compared to **0.9228** for LASSO.
  - LASSO demonstrated better performance, with lower error metrics and a higher \(R^2\) value compared to Random Forest.

### Key Findings
1. Random Forest is more suitable for prediction due to its higher accuracy and ability to model complex interactions.
2. LASSO is preferred for prediction due to its simplicity and better performance for this specific task.


## Getting Started
### Prerequisites
- Python 3.8+
- Required libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`
