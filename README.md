# SVM Classification with Anomaly Detection and Poisoning Attacks

## Overview

This project demonstrates the use of Support Vector Machines (SVM) for classification on the MNIST dataset, along with techniques for detecting and handling poisoned data. It includes implementations of label flipping and data injection attacks and evaluates the performance of the SVM model with and without anomaly detection using Isolation Forest.

## Features

- **Data Loading and Preprocessing**: Fetches and preprocesses the MNIST dataset, including scaling, normalization, and PCA.
- **Attack Simulations**: Implements label flipping and data injection attacks to simulate data poisoning.
- **Anomaly Detection**: Uses Isolation Forest to detect and remove poisoned data.
- **Model Training and Evaluation**: Trains SVM models and evaluates their performance using metrics such as accuracy, precision, recall, and F1-score.
- **Visualization**: Plots Precision-Recall curves, Confusion Matrices, Decision Boundaries (for 2D feature spaces), and ROC curves. Includes bar plots comparing accuracies across different scenarios.

## Requirements

- Python 3.x
- NumPy
- Matplotlib
- scikit-learn
- SciPy

You can install the required packages using pip:

```bash
pip install numpy matplotlib scikit-learn scipy


## Usage

1. **Load and Preprocess Data**:
   - Fetches the MNIST dataset and applies scaling, normalization, and PCA.

2. **Simulate Attacks**:
   - **Label Flipping Attack**: Randomly flips a proportion of labels.
   - **Data Injection Attack**: Injects noisy samples with altered labels.

3. **Train and Evaluate SVM**:
   - Train SVM models with and without anomaly detection.
   - Evaluate models using accuracy, precision, recall, and F1-score.

4. **Visualize Results**:
   - View Precision-Recall curves, Confusion Matrices, Decision Boundaries (for 2D data), and ROC curves.
   - Compare model accuracies in different scenarios using bar plots.

## Example

To run the analysis and generate plots, execute the script:

```bash
python svm_poisoning_detection.py
```

## Code Explanation

- **Data Loading and Preprocessing**: `load_and_preprocess_data` function handles data fetching, scaling, normalization, and PCA transformation.
- **Poisoning Attacks**: Functions `label_flipping_attack` and `data_injection_attack` simulate different types of data poisoning.
- **Anomaly Detection**: The `remove_poisoned_data` function uses Isolation Forest to clean the training data.
- **Model Training and Evaluation**: The `train_and_evaluate_svm` function trains the SVM model and evaluates its performance on test data.
- **Visualization**: Generates various plots to visualize model performance and results.



## Acknowledgments

- **MNIST Dataset**: Provided by [OpenML](https://www.openml.org/d/554).
- **Isolation Forest**: Anomaly detection algorithm used for identifying outliers.

```
