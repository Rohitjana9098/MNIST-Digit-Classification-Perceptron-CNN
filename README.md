# 🧠 MNIST Handwritten Digit Classification using Perceptron & CNN

An end-to-end Machine Learning & Deep Learning project evaluating and comparing a **Single-Layer Perceptron** baseline model against a multi-layer **Convolutional Neural Network (CNN)** for handwritten digit recognition on the MNIST dataset using TensorFlow/Keras.

---

## 📌 Project Overview

This repository demonstrates the power of Convolutional Neural Networks (CNNs) in spatial feature extraction compared to traditional linear single-layer Perceptrons for computer vision tasks:

- **Perceptron Model**: Simple single-layer neural network with Softmax activation.
- **CNN Model**: Deep architecture utilizing Conv2D layers, Max Pooling, Flattening, Dense layers, and Dropout regularization.

---

## 🏗️ Architecture & Model Comparison

| Feature / Metric | Single-Layer Perceptron | Convolutional Neural Network (CNN) |
| :--- | :--- | :--- |
| **Input Shape** | `(28, 28)` (Flattened to 784) | `(28, 28, 1)` (Spatial grid with channels) |
| **Feature Extraction** | None (Linear projection) | 2x Conv2D + 2x MaxPooling2D |
| **Regularization** | None | Dropout (0.5) |
| **Optimizer** | SGD (Stochastic Gradient Descent) | Adam |
| **Loss Function** | Categorical Cross-Entropy | Categorical Cross-Entropy |
| **Output Layer** | Dense (10 units, Softmax) | Dense (10 units, Softmax) |

---

## 📁 Repository Structure

```
.
├── CNN.ipynb          # Jupyter Notebook with code, output plots & training logs
├── CNN.py             # Python script implementation
├── requirements.txt   # Dependencies & libraries required
└── README.md          # Project documentation
```

---

## 📊 Workflow & Steps

1. **Data Preprocessing**:
   - Rescaling pixel values from `[0, 255]` to `[0.0, 1.0]`.
   - Reshaping input matrices for Perceptron `(28, 28)` vs CNN `(28, 28, 1)`.
   - One-hot encoding numeric labels into 10 target classes (`to_categorical`).

2. **Model Training & Evaluation**:
   - Models trained over 5 epochs with batch size 32.
   - Validation performance monitored on test split.
   - Loss and Accuracy curves plotted using Matplotlib.

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Rohitjana9098/MNIST-Handwritten-Digit-Classification-CNN.git
cd MNIST-Handwritten-Digit-Classification-CNN
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Execute script or notebook
Run Python script:
```bash
python CNN.py
```
Or open notebook:
```bash
jupyter notebook CNN.ipynb
```

---

## 🏷️ Suggested Repository Rename
Recommended repository name based on project contents:
👉 **`MNIST-Handwritten-Digit-Classification-CNN`** or **`MNIST-Digit-Classification-CNN`**
