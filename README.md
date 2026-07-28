# ML Analysis of the Relationship Between Electric Vehicle Charging Infrastructure, House Prices, and Air Quality in the United States

This repository contains the implementation, processed dataset, and final report for the project:

**"ML Analysis of the Relationship Between Electric Vehicle Charging Infrastructure, House Prices, and Air Quality in the United States"**

## Project Overview

The objective of this project is to investigate whether the presence of electric vehicle (EV) charging infrastructure is associated with:

- Residential property values
- Air quality (NO₂ concentrations)

at the county level across the United States during **2023–2025**.

The project integrates multiple public datasets, performs extensive preprocessing and feature engineering, and evaluates machine learning models for two prediction tasks.

---

## Repository Contents

### `MergeDatasets_EDA.ipynb`

This notebook performs the complete data preparation pipeline.

It includes:

- Loading all raw datasets
- Cleaning and preprocessing
- Geographic integration using county FIPS codes
- Feature engineering
- Missing-value evaluation
- Outlier detection
- Exploratory Data Analysis (EDA)
- Creation of the final modelling dataset
- Correlation analysis
- Variance Inflation Factor (VIF)

**Output:**

- `final_dataset_fixed.csv`

---

### `ML_Evaluation.ipynb`

This notebook contains the complete machine learning workflow.

It includes:

- Feature selection
  - Mutual Information
  - Recursive Feature Elimination with Cross-Validation (RFECV)
- Model training
  - Linear Regression
  - XGBoost
- Hyperparameter optimization using GridSearchCV
- GroupKFold cross-validation
- Test-set evaluation
- SHAP feature importance analysis
- Generation of all figures used in the final report

---

### `final_dataset_fixed.csv`

The final processed dataset used throughout the project.

The dataset contains county-level observations for **2023–2025**, including:

- EV charging infrastructure
- Housing prices
- Air pollution (NO₂)
- Transportation variables
- Demographic characteristics
- Engineered features used for model training

This dataset serves as the input for all machine learning analyses.

---

### `FinalReport_324239284_325390201.pdf`

The final project report describing:

- Research motivation
- Data sources
- Data integration and preprocessing
- Machine learning methodology
- Feature selection
- Model evaluation
- SHAP explainability analysis
- Results, discussion, and conclusions

---

## Machine Learning Models

The following models were evaluated:

- Linear Regression
- XGBoost

Model performance was assessed using:

- GroupKFold Cross-Validation
- Train/Test Split (2023–2024 → 2025)
- R²
- MAE
- RMSE

---

## Explainability

Model interpretation was performed using:

- SHAP Feature Importance
- SHAP Beeswarm Plots
- Standardized Linear Regression Coefficients

---

## Authors

- **Riham Badarna**
- **Mira Bitar**

Information Systems Department  
University of Haifa
