# astronomical-object-classification
Astronomical Object Classification using Computer Vision
Overview

This project implements a deep learning system for classifying astronomical objects from images using Computer Vision techniques and transfer learning.

The model is based on a pre-trained ResNet18 architecture and fine-tuned on a custom dataset of astronomical object images. The system performs automatic image classification and provides detailed evaluation metrics and visualizations of model performance.

Project Goals
Develop an image classification system for astronomical objects.
Apply transfer learning using a pre-trained convolutional neural network.
Improve model generalization through data augmentation.
Evaluate classification quality using standard machine learning metrics.
Technologies
Python
PyTorch
NumPy
Pandas
Matplotlib
Seaborn
PIL (Pillow)
Scikit-learn
Model Architecture

The project uses:

ResNet18 pre-trained on ImageNet
Transfer Learning
Fine-tuning of the final layers
Dropout regularization
AdamW optimizer
Cosine Annealing Learning Rate Scheduler
Early Stopping
Dataset Processing

The dataset is automatically loaded from class-specific folders.

Data preprocessing includes:

Image resizing
Normalization
Random cropping
Horizontal and vertical flipping
Random rotation
Color augmentation
Random affine transformations
Perspective transformations

These techniques help reduce overfitting and improve model robustness.

Training Pipeline
Dataset loading and preprocessing.
Stratified train/validation/test split.
Data augmentation.
Model initialization with pre-trained weights.
Fine-tuning using transfer learning.
Validation during training.
Early stopping to prevent overfitting.
Final evaluation on the test dataset.
Evaluation Metrics

The model is evaluated using:

Accuracy
Precision
Recall
F1-Score
Classification Report

Additional visualizations include:

Training and validation loss curves
Accuracy curves
Learning rate schedule
Overfitting analysis (Train-Val Gap)
Prediction examples on test images
