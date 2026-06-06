# Handwritten Digit Recognition using CNN

A Convolutional Neural Network (CNN) built from scratch in Python to classify handwritten digits (0-9) using the MNIST dataset. Developed as part of the AI202L Artificial Intelligence Lab course at Ghulam Ishaq Khan Institute (GIKI).

---

## Overview

This project implements a CNN for image classification, covering the full pipeline from data loading and preprocessing through model architecture, training, evaluation, and visualization of results. The goal was to build an understanding of deep learning fundamentals — convolutional layers, pooling, dropout, and backpropagation — by applying them to a real classification task.

---

## What It Covers

- Loading and preprocessing the MNIST dataset (60,000 training / 10,000 test images)
- Normalizing pixel values and reshaping inputs for CNN compatibility
- Building a CNN architecture with convolutional, pooling, dropout, and dense layers
- Training the model and tracking accuracy and loss across epochs
- Evaluating performance on the test set
- Visualizing predictions, confusion matrix, and training curves

---

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Python |
| Deep learning | TensorFlow / Keras |
| Data | MNIST (via Keras datasets) |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## Model Architecture

```
Input (28x28x1)
    → Conv2D + ReLU
    → MaxPooling2D
    → Conv2D + ReLU
    → MaxPooling2D
    → Dropout
    → Flatten
    → Dense (ReLU)
    → Dense (Softmax, 10 classes)
```

---

## Setup

**1. Clone the repository**

```bash
git clone https://github.com/09Rumaisa/number_recognition-using-CNN.git
cd number_recognition-using-CNN
```

**2. Install dependencies**

```bash
pip install tensorflow numpy matplotlib seaborn jupyter
```

**3. Run the notebook**

```bash
jupyter notebook "AI202L_Proj (2).ipynb"
```

---

## Dataset

MNIST — 70,000 grayscale images of handwritten digits (28x28 pixels), 10 classes (0-9). Loaded directly via `tensorflow.keras.datasets.mnist` — no manual download required.

---

## Files

```
number_recognition-using-CNN/
└── AI202L_Proj (2).ipynb    # Full notebook: data loading, model, training, evaluation
```

---

## Context

This was completed as a lab project for AI202L (Artificial Intelligence Lab) at GIKI, focusing on hands-on implementation of deep learning concepts covered in the course. It demonstrates understanding of CNN architecture design, training loops, regularization with dropout, and evaluation with classification metrics.

---

## Author

Rumaisa Siddiqa
GitHub: https://github.com/09Rumaisa
LinkedIn: https://linkedin.com/in/rumaisa-siddiqa
