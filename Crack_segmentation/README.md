# 🔍 Crack Segmentation on Asphalt Photos using Deep Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-red)

## 📋 Project Overview

This project implements a deep learning solution to detect and classify cracks in asphalt and concrete surfaces. Using convolutional neural networks (CNNs), we've created an automated system that can identify the presence of cracks in images with high accuracy, precision, and recall.

## 🌟 Key Features

- **Binary classification model**: Identifies presence or absence of cracks in photos
- **Data augmentation pipeline**: Enhances model generalization capabilities
- **Hyperparameter tuning**: Optimized model architecture using keras-tuner
- **Advanced visualization**: Used saliency maps to explain model decisions
- **High accuracy**: Achieved 95% test accuracy with strong precision and recall

## 🛠️ Technical Implementation

### Data Preparation
- Split data into training (80%) and validation (20%) sets
- Created robust data augmentation pipeline 

### Model Architecture Search
Used keras-tuner to find the optimal network architecture


## 📊 Results

Final model achieved impressive metrics on the test set:

- **Accuracy**: 94.99%
- **AUC**: 96.65%
- **Precision**: 95.90%
- **Recall**: 98.44%

### Performance Visualization

![Model Training Performance](https://github.com/Bialkasss/DeepLearning/blob/01fe8d7946514fb0e983681a0476a4eca1270232/Crack_segmentation/performance.png)

The model showed strong convergence with minimal overfitting after implementing early stopping and model checkpointing.


## 🔬 Explainable AI

We implemented saliency maps to understand what features the model focuses on when making predictions:

![Saliency Maps](https://github.com/Bialkasss/DeepLearning/blob/01fe8d7946514fb0e983681a0476a4eca1270232/Crack_segmentation/output.png)

Key insights:
- For crack images: The model correctly focuses on the actual crack regions
- For non-crack images with tiles: The model identifies the grid pattern of tiles
- The model learned to ignore image borders effectively

## 👩‍💻 Authors

- Maria Musiał
