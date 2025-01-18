# Comparison-of-two-ML-algorithms-to-compute-optical-properties-of-photonic-crystal-fiber

This project explores the use of machine learning to predict key optical properties of photonic crystal fibers (PCFs), including the **effective index** (\(n_{\text{eff}}\)) and **effective mode area** (\(A_{\text{eff}}\)).

## Overview
Photonic crystal fibers (PCFs) are critical in various optical applications due to their unique properties. This study leverages two machine learning models, **LASSO** and **Random Forest**, to predict \(n_{\text{eff}}\) and \(A_{\text{eff}}\) based on PCF design parameters.

## Machine Learning Models
The following machine learning models were employed:
- **LASSO (Least Absolute Shrinkage and Selection Operator):** Effective for sparse feature selection and linear relationships.
- **Random Forest:** A robust ensemble learning method capable of capturing complex relationships.

## Dataset
The models were trained on a synthetic dataset of PCF parameters:
- **Wavelength:** \(0.5–1.8 \, \mu\text{m}\)
- **Pitch:** \(0.8–2.0 \, \mu\text{m}\)
- **Diameter-to-pitch ratio:** \(0.6–0.9\)
- **Number of air hole rings:** 4 or 5

## Performance Metrics
The performance of the models was evaluated using:
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **R-squared (\(R^2\))**

## Results
- **\(n_{\text{eff}}\) Prediction:**
  - Random Forest outperformed LASSO with an \(R^2\) value of **0.99** compared to **0.9228** for LASSO.
- **\(A_{\text{eff}}\) Prediction:**
  - LASSO demonstrated better performance, with lower error metrics and a higher \(R^2\) value compared to Random Forest.

### Key Findings
1. Random Forest is more suitable for \(n_{\text{eff}}\) prediction due to its higher accuracy and ability to model complex interactions.
2. LASSO is preferred for \(A_{\text{eff}}\) prediction due to its simplicity and better performance for this specific task.

## Repository Contents
- **`notebooks/`:** Contains the Colab notebook with code for training and evaluation.
- **`data/`:** Synthetic dataset used for the study.
- **`results/`:** Summary of model evaluation metrics and visualizations.
- **`README.md`:** Overview of the project.

## Getting Started
### Prerequisites
- Python 3.8+
- Required libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`
