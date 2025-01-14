# Handwritten Character Recognition Using CNN

## Overview
This project implements a **Convolutional Neural Network (CNN)** to recognize handwritten characters using the EMNIST Balanced dataset. The goal is to classify characters into one of 47 categories, including uppercase letters, lowercase letters, and digits.
---

## Features
- **Model Architecture**: A CNN model with convolutional, pooling, and fully connected layers optimized for feature extraction and classification.
- **Dataset**: EMNIST Balanced dataset.
- **Performance Metrics**: Accuracy, precision, recall, and F1-score.
- **Visualization**: Training and validation loss/accuracy curves.
---

## Dataset
### EMNIST Balanced Dataset
The EMNIST Balanced dataset contains handwritten digits and characters. It is derived from the NIST Special Database 19 and is compatible with the MNIST dataset format.

- **Number of Classes**: 47 (digits [0-9], uppercase letters [A-Z], lowercase letters [a-z] with similar forms merged).
- **Training Samples**: 112,800
- **Testing Samples**: 18,800
- **Input Format**: 28x28 grayscale images.

# Download and load the dataset
train_set = datasets.EMNIST(root='./data', split='balanced', train=True, download=True, transform=transform)
test_set = datasets.EMNIST(root='./data', split='balanced', train=False, download=True, transform=transform)
