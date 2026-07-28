# Intrusion Detection System using PyTorch

A deep learning-based **Intrusion Detection System (IDS)** developed using **PyTorch** and the **UNSW-NB15** dataset. This project implements a Multi-Layer Perceptron (MLP) to classify normal and malicious network traffic through data preprocessing, model training, threshold tuning, and performance evaluation.

---

## Project Overview

Cybersecurity threats continue to evolve, making automated intrusion detection an essential part of modern network security. This project applies a neural network model to detect malicious network traffic using the UNSW-NB15 benchmark dataset.

The workflow includes:

* Data preprocessing and feature engineering
* Categorical feature encoding
* Feature scaling
* Training an MLP using PyTorch
* Model evaluation using multiple metrics
* Prediction on unseen test data

---

## Dataset

This project uses the **UNSW-NB15** dataset, a widely used benchmark dataset for network intrusion detection research.

The dataset contains both normal and attack network traffic with multiple numerical and categorical features.

**Files used**

* Training dataset
* Testing dataset
* Unlabeled testing dataset for predictions

---

## Technologies Used

* Python
* PyTorch
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Google Colab / Jupyter Notebook

---

## Model Architecture

The implemented Multi-Layer Perceptron consists of:

* Input Layer
* Hidden Layer 1 (ReLU)
* Dropout
* Hidden Layer 2 (ReLU)
* Dropout
* Output Layer

Training includes:

* Adam Optimizer
* BCEWithLogitsLoss
* Threshold tuning for improved classification performance

---

## Performance

The optimized model achieved approximately:

| Metric    | Score     |
| --------- | --------- |
| Accuracy  | **91.7%** |
| Precision | **97.4%** |
| Recall    | **90.0%** |
| F1 Score  | **93.6%** |

These results demonstrate strong performance in identifying malicious network traffic while maintaining high precision.

---

## Repository Structure

```
intrusion-detection-system-pytorch/
│
├── Intrusion_Detection_MLP_PyTorch.ipynb
├── requirements.txt
├── README.md
├── results/
│   └── UNSWNB15_testing2_predictions.csv
└── images/
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/intrusion-detection-system-pytorch.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook using Jupyter Notebook or Google Colab.

---

## Future Improvements

* Compare multiple deep learning architectures
* Hyperparameter optimization
* Explainable AI techniques (SHAP/LIME)
* Real-time intrusion detection
* Deployment using Flask or FastAPI

---

## Disclaimer

This project is intended for educational and research purposes. The UNSW-NB15 dataset is publicly available for academic use. Please ensure compliance with the dataset's licensing terms when redistributing data.
