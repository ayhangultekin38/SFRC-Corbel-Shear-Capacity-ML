# SFRC Corbel Shear Capacity Prediction

## Overview

This repository provides the dataset, reproducibility notebook,
and browser-based prediction tool associated with the study:

"Source-Study-Aware Validation and Explainable Machine Learning
for Reliable Shear Capacity Assessment of Steel-Fiber-Reinforced
Concrete Corbels"

The database contains 108 specimens collected from seven
independent experimental source studies.

## Models

Three regression models are included:

- Linear Regression
- Ridge Regression
- XGBoost

## Input Variables

- a/d
- b
- rho
- fy
- fc
- ff
- Vf

## Repository Contents

- Corbel_Dataset.xlsx — dataset used in the study
- Corbel_Reproducibility.ipynb — complete analysis notebook
- Corbel_Shear_Capacity_Calculator.html — browser-based calculator
- requirements.txt — software dependencies

## Reproducibility

The analysis was performed using Python 3.12.13.

Hyperparameter selection for Ridge Regression and XGBoost was
performed using nested, source-study-aware GroupKFold
cross-validation within each outer training set.

## Browser-Based Calculator

The calculator can be used without installing Python.

Download:

Corbel_Shear_Capacity_Calculator.html

and open the file in a modern web browser.

The tool provides predictions from Linear Regression,
Ridge Regression, and XGBoost.

Input values outside the parameter ranges represented in the
database generate an extrapolation warning.

## Important Limitation

The models are intended for research and preliminary
decision-support purposes within the parameter ranges represented
in the database.

They should not be interpreted as general-purpose structural
design equations or substitutes for applicable design codes.

## Data and Code Availability

All data and code required to reproduce the analyses reported in
the manuscript are provided in this repository.

## Citation

Citation information will be updated following publication of the article.
