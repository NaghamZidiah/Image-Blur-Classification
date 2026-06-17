# Image Blur Classification

## Overview

This project focuses on classifying images into two categories: Sharp and Blurred.

The proposed approach combines image processing techniques with machine learning by extracting meaningful image quality features and using them as input for a Multi-Layer Perceptron (MLP) neural network.

The objective is to automatically detect image blur caused by motion or focus issues and evaluate the effectiveness of neural networks for image quality assessment.

## Google Colab Notebook

You can explore and run the project directly in Google Colab:

https://colab.research.google.com/drive/1iIzINr4nGBCYTjZnJyM5G63GGEcZ7ocd?usp=sharing

## Project Report

The complete project report is available in the `reports` folder.

## Project Presentation

The project presentation slides are available in the `presentation` folder.

## Dataset

The dataset contains three image categories:

- Sharp Images
- Motion Blur Images
- Defocus Blur Images

For the classification task, motion blur and defocus blur images were combined into a single Blur class, while sharp images remained as a separate class.

The dataset subset used in the project included:

- 300 Sharp Images
- 300 Motion Blur Images
- 300 Defocus Blur Images

## Preprocessing

- Image resizing (256 × 256)
- Grayscale conversion
- Feature normalization using StandardScaler

## Feature Extraction

Several handcrafted image features were extracted:

- Variance of Laplacian
- Tenengrad (Sobel Gradient Magnitude)
- Image Contrast
- High-Frequency Energy (FFT)

These features were used as inputs to the neural network.

## Model Architecture

A Multi-Layer Perceptron (MLP) classifier was implemented with:

- Input Layer (4 Features)
- Two Hidden Layers with ReLU Activation
- Output Layer for Binary Classification

## Experiments

Two optimization algorithms were evaluated:

### Adam Optimizer

- Accuracy: 94%
- Stable convergence
- Best overall performance

### SGD Optimizer

- Accuracy: 91%
- Slightly lower performance compared to Adam

## Results

The experimental results demonstrated that handcrafted image features combined with neural networks can effectively distinguish between sharp and blurred images.

The Adam optimizer achieved the highest classification accuracy and produced the most reliable predictions.

## Technologies Used

- Python
- OpenCV
- NumPy
- Scikit-Learn
- TensorFlow
- Keras
- Matplotlib

## Author

**Nagham Zidiah**

Data Science & Artificial Intelligence Student

Palestine Technical University – Kadoorie
