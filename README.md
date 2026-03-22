# breast-tissue-classification
Overview
This project implements a deep learning-based classification system for breast tissue analysis using the BreastMNIST dataset. The model is designed to classify tissue samples as either benign or malignant, providing a tool to assist in medical diagnostics.

This project was developed as part of a technical interview for a recruitment process, demonstrating skills in deep learning, computer vision, and end-to-end machine learning pipeline development.

Dataset
The project utilizes the BreastMNIST dataset, which is part of the MedMNIST collection - a large-scale MNIST-like collection of standardized biomedical images. The dataset consists of:

Image size: 28×28 pixels

Channels: Grayscale

Classes: 2 (Benign and Malignant)

Split:

Training: Pre-defined split

Validation: Pre-defined split

Testing: Pre-defined split

Model Architecture
The implemented Convolutional Neural Network (CNN) architecture consists of:

First Convolutional Block:

Conv2D: 64 filters, 3×3 kernel, ReLU activation

BatchNormalization

MaxPooling2D: 2×2 pool size

Dropout: 0.25

Second Convolutional Block:

Conv2D: 128 filters, 3×3 kernel, ReLU activation

BatchNormalization

MaxPooling2D: 2×2 pool size

Dropout: 0.25

Fully Connected Layers:

Flatten

Dense: 128 units, ReLU activation

BatchNormalization

Dropout: 0.5

Output: Dense with 1 unit, Sigmoid activation
