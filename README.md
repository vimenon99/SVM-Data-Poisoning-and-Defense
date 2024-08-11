

```markdown
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
```

## Usage

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Dependencies**:
   ```bash
   pip install numpy matplotlib scikit-learn scipy
   ```

3. **Run the Script**:
   Execute the main script to perform data loading, attack simulation, model training, and visualization:
   ```bash
   python svm_poisoning_detection.py
   ```

4. **Review Results**:
   The script will output performance metrics including accuracy, precision, recall, and F1-score. It will also generate visualizations such as Precision-Recall curves, Confusion Matrices, Decision Boundaries (for 2D feature spaces), and ROC curves.

## Code Explanation

- **Data Loading and Preprocessing**:
  - `load_and_preprocess_data()`: Loads the MNIST dataset and applies scaling, normalization, and PCA.

- **Poisoning Attacks**:
  - `label_flipping_attack()`: Simulates label flipping by modifying a portion of the labels.
  - `data_injection_attack()`: Injects noisy samples with altered labels to simulate data injection attacks.

- **Anomaly Detection**:
  - `remove_poisoned_data()`: Uses Isolation Forest to identify and remove poisoned data.

- **Model Training and Evaluation**:
  - `train_and_evaluate_svm()`: Trains the SVM model and evaluates its performance on the dataset.

- **Visualization**:
  - Generates and displays Precision-Recall curves, Confusion Matrices, Decision Boundaries (for 2D data), and ROC curves.
  - Compares accuracies across different attack scenarios using bar plots.



## Acknowledgments

- **MNIST Dataset**: Sourced from [OpenML](https://www.openml.org/d/554).
- **Isolation Forest**: Utilized for anomaly detection to identify outliers in the data.
```
