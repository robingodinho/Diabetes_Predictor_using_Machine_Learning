# Diabetes Prediction using Machine Learning

A machine learning project that predicts diabetes diagnosis using the Pima Indians Diabetes Dataset. This project demonstrates data preprocessing, feature selection, model training, and evaluation using logistic regression.
![Data_Analysis]()

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Future Improvements](#future-improvements)
- [License](#license)

## Overview

This project builds a predictive model to determine whether a patient has diabetes based on various health measurements. The workflow includes:
- Data loading and exploratory analysis
- Feature selection using correlation and variance thresholding
- Data visualization
- Model training using Logistic Regression
- Model evaluation with multiple metrics

## Dataset

The **Pima Indians Diabetes Dataset** contains medical records from adult female patients of Pima Indian heritage. 

### Features:
- **Pregnancies**: Number of pregnancies
- **Glucose**: Plasma glucose concentration (2-hour oral glucose tolerance test)
- **BloodPressure**: Diastolic blood pressure (mm Hg)
- **SkinThickness**: Triceps skinfold thickness (mm)
- **Insulin**: 2-hour serum insulin (μU/ml)
- **BMI**: Body mass index (weight in kg/(height in m)²)
- **DiabetesPedigreeFunction**: Genetic predisposition score
- **Age**: Age in years
- **Outcome**: Binary target (0 = no diabetes, 1 = diabetes)

Dataset source: [Kaggle - Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

## Features

### Data Preprocessing
- Missing value analysis
- Correlation-based feature selection (threshold > 0.1)
- Variance threshold filtering (threshold = 0.01)
- Data standardization using StandardScaler

### Model Training
- Train-test split (80/20)
- Logistic Regression with 1000 max iterations
- Random state = 64 for reproducibility

### Evaluation Metrics
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)

## Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/diabetes-prediction.git
cd diabetes-prediction

# Install required packages
pip install pandas numpy scikit-learn matplotlib seaborn
