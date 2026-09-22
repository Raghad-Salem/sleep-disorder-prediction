# Sleep Health and Sleep Disorder Prediction

## Project Overview

This project explores patterns related to sleep health and sleep disorders using data analysis and machine learning.

The main goal is to investigate whether sleep, lifestyle, and health-related variables can help distinguish between different sleep disorder categories.

## Problem

Sleep disorders can be associated with multiple factors such as sleep duration, sleep quality, stress, physical activity, age, and other health-related variables.

This project investigates the following question:

> Can sleep, lifestyle, and health information be used to predict sleep disorder categories?

## Dataset

The dataset contains information about sleep health and lifestyle, including:

- Gender
- Age
- Occupation
- Sleep Duration
- Quality of Sleep
- Physical Activity Level
- Stress Level
- BMI Category
- Heart Rate
- Daily Steps
- Blood Pressure
- Sleep Disorder

The target variable is `Sleep Disorder`, with three categories:

- No Disorder
- Insomnia
- Sleep Apnea

The dataset is synthetic, so the findings should not be generalized directly to real-world clinical populations.

## Methodology

The project followed a structured data science workflow:

1. Data Understanding
2. Variable Understanding
3. Exploratory Data Analysis
4. Hypothesis Investigation
5. Feature Preparation
6. Machine Learning
7. Interpretation and Practical Implications

## Exploratory Data Analysis

The analysis investigated relationships between sleep disorders and:

- Age
- Sleep Duration
- Quality of Sleep
- Stress Level
- Physical Activity Level

Strong relationships were also observed between Sleep Duration, Quality of Sleep, and Stress Level.

## Data Preparation

The `Blood Pressure` variable was transformed into two numerical features:

- Systolic BP
- Diastolic BP

`Person ID` was excluded because it is an identifier rather than a meaningful predictive feature.

Categorical variables were encoded and numerical variables were standardized before modeling.

## Machine Learning

A Logistic Regression model was used to predict the `Sleep Disorder` category.

A majority-class baseline was also used for comparison.

### Results

- Baseline Accuracy: 57.33%
- Logistic Regression Test Accuracy: 90.67%
- Mean 5-Fold Cross-Validation Accuracy: 90.63%

The model performed differently across the three sleep-disorder classes, so precision, recall, and F1-score were also considered.

## Interpretation

The results show that the variables in this dataset contain useful patterns for distinguishing between sleep disorder categories.

The model is intended as an exploratory data science project and should not be considered a medical diagnostic tool.

## Limitations

- The dataset is synthetic.
- The dataset is relatively small.
- Observed relationships represent associations and do not establish causation.
- Model performance on this dataset does not guarantee the same performance on real-world clinical data.

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- GitHub

## Author

Raghad Salem
