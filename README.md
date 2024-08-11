

```markdown
# SVM with Anomaly Detection on MNIST

This project demonstrates the use of Support Vector Machines (SVM) with and without anomaly detection on the MNIST dataset. It explores the impact of label flipping and data injection attacks on SVM performance and evaluates the effectiveness of Isolation Forest for anomaly detection.

## Installation

Install the required libraries using:

```bash
pip install numpy matplotlib scikit-learn scipy
```

## Usage

1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Run the script:

    ```bash
    python svm_anomaly_detection.py
    ```

## Features

- **Data Preparation**: Loads and preprocesses the MNIST dataset (scaling, normalization, PCA).
- **Attacks**: Simulates label flipping and data injection attacks.
- **Evaluation**: Trains SVM with and without anomaly detection (Isolation Forest).
- **Metrics**: Displays accuracy, precision, recall, F1-score, confusion matrix, ROC, and Precision-Recall curves.

## Results

The script provides:
- Performance metrics and confusion matrix for standard and anomaly-detected SVM.
- Bar plots comparing SVM accuracy under different conditions.

## Dependencies

- Python 3.x
- `numpy`
- `matplotlib`
- `scikit-learn`
- `scipy`

