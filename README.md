# Breast Tissue Classification - End-to-End Platform

## Overview

This project implements a deep learning-based classification system for breast tissue analysis using the BreastMNIST dataset. The model is designed to classify tissue samples as either benign or malignant.
This project was developed as part of a technical interview for a recruitment process of Junior AI.
## Dataset

The project utilizes the **BreastMNIST** dataset, which is part of the MedMNIST collection - a large-scale MNIST-like collection of standardized biomedical images. The dataset consists of:
- **Image size**: 28×28 pixels
- **Channels**: Grayscale
- **Classes**: 2 (Benign and Malignant)
- **Split**:
  - Training: Pre-defined split
  - Validation: Pre-defined split
  - Testing: Pre-defined split

## Model Architecture
The implemented Convolutional Neural Network (CNN) architecture consists of:
### First Convolutional Block
- Conv2D: 64 filters, 3×3 kernel, ReLU activation
- BatchNormalization
- MaxPooling2D: 2×2 pool size
- Dropout: 0.25
### Second Convolutional Block
- Conv2D: 128 filters, 3×3 kernel, ReLU activation
- BatchNormalization
- MaxPooling2D: 2×2 pool size
- Dropout: 0.25
### Fully Connected Layers
- Flatten
- Dense: 128 units, ReLU activation
- BatchNormalization
- Dropout: 0.5
- Output: Dense with 1 unit, Sigmoid activation

### Model Summary
## Performance Metrics

The model is evaluated using multiple metrics:

- **Accuracy** - 0.8013
- **Precision** - 0.8217
- **Recall** - 0.9298
- **F1 Score** - 0.8444
- **Loss** - 0.4468

## Technical Stack
- **Framework**: TensorFlow / Keras
- **Data Handling**: NumPy, Pandas
- **Visualization**: Matplotlib, Seaborn
- **Dataset Loading**: MedMNIST
- **Model Evaluation**: Scikit-learn metrics

## Key Features
- End-to-end pipeline from data loading to model evaluation
- Data preprocessing and normalization
- CNN model with batch normalization and dropout for regularization
- Comprehensive evaluation metrics and visualizations
- Confusion matrix visualization
- Sample predictions visualization with confidence scores

## Usage
The notebook can be run in Google Colab or locally with the required dependencies installed.

