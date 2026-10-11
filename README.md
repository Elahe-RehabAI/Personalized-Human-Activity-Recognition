# Personalized Human Activity Recognition

## Overview

This project investigates whether personalization can improve Human Activity Recognition (HAR) using smartphone sensor data.

A Logistic Regression model is used as a baseline classifier to recognize six daily activities. The project also explores whether incorporating subject-specific data can improve model performance for individual users.

## Research Question

**Can personalization improve human activity recognition for individual users?**

## Dataset

The project uses the [Human Activity Recognition with Smartphones dataset](https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones).

- 30 participants
- 6 activity classes
- Accelerometer and gyroscope features
- 50 Hz sampling frequency
- 561 sensor-based features

Activities:
- Walking
- Walking Upstairs
- Walking Downstairs
- Sitting
- Standing
- Laying

## Methods

- Data exploration and preparation
- Logistic Regression baseline
- Random Forest comparison
- Classification metrics and confusion matrix analysis
- Feature importance analysis
- 5-fold cross-validation
- Subject-specific performance analysis
- Personalized model training
- Wilcoxon signed-rank test
- Personalization data-size and robustness experiments

## Key Results

- Logistic Regression achieved **96.17% test accuracy**.
- Random Forest achieved **92.60% test accuracy**.
- For Subject 10, accuracy improved from **86.4% to 97.3%** after personalization.
- Mean accuracy across nine test subjects increased from **95.9% to 98.2%**.
- Increasing the amount of personalization data generally improved performance.

The Wilcoxon signed-rank test yielded **p = 0.0625**. Therefore, the overall improvement was not statistically significant at the conventional 0.05 level.

## Limitations

- The personalization experiment covered only nine test subjects.
- Personalization was evaluated in a simulated adaptation setting.
- Logistic Regression was used for the personalization experiments.
- The results require further validation using a more rigorous experimental protocol.

## Future Work

- Explore deep learning models such as CNNs and LSTMs.
- Investigate transfer learning and alternative personalization strategies.
- Evaluate models using more subjects and rigorous subject-independent protocols.
- Extend the project toward real-time, context-aware assistive systems.

## Technologies

- Python
- Pandas
- Matplotlib
- Scikit-learn
- SciPy
- Jupyter Notebook
- Kaggle

## Project Goal

The long-term goal is to investigate how personalized activity recognition can support context-aware and adaptive assistive technologies.
