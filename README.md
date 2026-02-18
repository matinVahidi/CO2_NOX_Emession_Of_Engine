# Thermodynamics Machine Learning Project

Sharif University of Technology  
Faculty of Aerospace Engineering  
Instructor: Mohammadreza Morad  
Author: Mohammad Matin Vahidi  
Farvardin 1403  

---

## Project Overview

This project explores the application of machine learning algorithms to predict **CO** and **NOX** emissions using thermodynamic dataset variables.  

The workflow includes:

- Environment setup and debugging
- Data preprocessing and cleaning
- Exploratory data analysis (EDA)
- Model selection and comparison
- Regression techniques (linear, polynomial, ridge, lasso)
- Neural networks
- Decision trees
- Model evaluation (R² and MSE)

---

# 1. Environment Setup

- Python (Jupyter Notebook)
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - scikit-learn
  - tensorflow

Several setup issues were resolved:
- Firewall restrictions
- Jupyter kernel mismatch
- Virtual environment configuration
- Missing libraries

---

# 2. Data Preprocessing (CO)

## 2.1 Initial Analysis

Selected variables:

- AT
- AP
- AH
- AFDP
- GTEP
- TIT
- TAT
- CDP
- TEY

Steps performed:

- Removed null values
- Merged yearly CSV files
- Histogram visualization
- Scatter plots for correlation inspection
- Train/Test split (80/20)

---

# 3. Model Experiments for CO

## 3.1 Simple Linear Regression (TIT → CO)

R² ≈ 0.50  

Moderate predictive capability.

---

## 3.2 Multiple Linear Regression

Variables:
- TEY
- CDP
- AFDP
- GTEP
- TIT

R² ≈ 0.57 – 0.60

Improvement over single-variable model
