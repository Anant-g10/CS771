# Binary Classification with Multi-Modal Features

## Overview
This project investigates a binary classification task using three distinct datasets, each offering a different feature representation of the same underlying problem. The objectives of this study were:

- To evaluate and compare model performance on each dataset individually
- To explore whether combining all feature representations improves performance
- To assess how much training data is necessary to achieve strong generalization

This project was completed as part of the CS771: Introduction to Machine Learning course at IIT Kanpur.

## Tasks and Methodology

### Task 1: Training on Individual Datasets
Each dataset was preprocessed and evaluated independently using a variety of machine learning models:

- Models: K-Nearest Neighbors, Logistic Regression, Random Forest, XGBoost, and LSTM
- Evaluation based on validation accuracy and generalization to unseen data
- Training proportions ranged from 20% to 100%

Best individual performance was achieved with logistic regression on deep features (98.7% accuracy).

### Task 2: Combined Feature Representation
In this task, all three datasets were merged by:
- Flattening deep features (13x768) and applying PCA for dimensionality reduction
- Vectorizing emoticon and text data using CountVectorizer
- Concatenating all feature sets into a unified matrix
- Training and evaluating a logistic regression model

Combining datasets did not significantly outperform the best individual model, indicating that some representations were more informative than others.

This repository is intended for academic use only.
