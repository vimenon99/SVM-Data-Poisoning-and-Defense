# SVM Classification with Anomaly Detection and Poisoning Attacks

## Overview

This project demonstrates the application of Support Vector Machines (SVM) for classification on the MNIST dataset, with a focus on detecting and handling poisoned data. It includes implementations of label flipping and data injection attacks and evaluates the performance of the SVM model with and without anomaly detection using Isolation Forest.

## Features

- **Data Loading and Preprocessing**: Retrieves and preprocesses the MNIST dataset, including scaling, normalization, and PCA.
- **Attack Simulations**: Simulates label flipping and data injection attacks to model data poisoning.
- **Anomaly Detection**: Utilizes Isolation Forest to detect and remove poisoned data.
- **Model Training and Evaluation**: Trains SVM models and assesses their performance using metrics such as accuracy, precision, recall, and F1-score.
- **Visualization**: Provides visualizations including Precision-Recall curves, Confusion Matrices, Decision Boundaries (for 2D feature spaces), and ROC curves. Compares accuracies across different scenarios with bar plots.

## Requirements

- Python 3.x
- NumPy
- Matplotlib
- scikit-learn
- SciPy

To install the required packages, run:

```bash
pip install numpy matplotlib scikit-learn scipy
