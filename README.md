This project demonstrates how to build and track Artificial Neural Network (ANN) models using **MLflow**. It focuses on tuning key hyperparameters — **learning rate** and **momentum** — and logging metrics, parameters, and model artifacts.

---

## 🚀 Project Overview

The goal is to evaluate the performance of ANN models across multiple combinations of learning rates and momentum values, using **MLflow** to:
- Log training/validation metrics
- Record hyperparameters
- Save trained models
- Visualize experiment results

## 🧠 Model Architecture

This project uses a **Keras Sequential model** for regression tasks. The model includes a normalization layer followed by two dense layers.

- **Input Layer:** Automatically shaped based on training data features
- **Normalization Layer:** Applies feature-wise normalization using the training set’s mean and variance
- **Hidden Layer:** 64 neurons with ReLU activation
- **Output Layer:** Single neuron for regression output

### ⚙️ Compilation Settings

- **Loss Function:** Mean Squared Error (`mean_squared_error`)
- **Optimizer:** Stochastic Gradient Descent (SGD)
  - Tunable `learning_rate` and `momentum`
- **Metric:** Root Mean Squared Error (RMSE)

### 🧪 Python Environment

- Python 3.10.10
- TensorFlow/Keras (>=2.10)
