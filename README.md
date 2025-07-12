# Skin Lesion Classification Using ResNet-based Models on HAM10000 Dataset

# 👀 Overview

This project focuses on developing deep learning models for skin lesion classification using the HAM10000 dataset, which consists of 10,015 dermoscopy images classified into seven distinct skin lesion groups. The main objective is to compare the performance of two ResNet-based architectures, ResNet50 and InceptionResNetV2, in two configurations: (A) training the entire model and (B) training only the newly added classifier layers. The project addresses data imbalance issues, improves the quality of the dataset through augmentation, and evaluates model performance using metrics such as accuracy, precision, recall, and F1 score.

# 🎯 Objectives
Dataset Construction: Prepare and augment the HAM10000 dataset to address class imbalance, ensuring each class contains 2,000 images (total: 14,000 images).
Data Preprocessing: Apply preprocessing and augmentation techniques to improve classification performance and handle data imbalance.
Model Development: Implement and compare ResNet50 and InceptionResNetV2 architectures with two configurations:
- Configuration (A): Fine-tune the entire model.
- Configuration (B): Train only the newly added classification layers.
Model Customization: Redesign the fully connected layers to suit the 7-class classification task.
Performance Evaluation: Analyze model performance using precision, recall, and F1-score, with a focus on performance across all classes, particularly those with fewer samples in the original dataset.

# 🗂️ Dataset
The HAM10000 dataset consists of 10,015 dermoscopic images of skin lesions, categorized into seven classes.
- Data Preprocessing
  - Imbalance Handling: The original dataset was highly imbalanced, with the nv class having 6,705 images and df and vasc having only 115 and 142 images, respectively. We applied seven data augmentation techniques (e.g., rotation, flipping, brightness adjustment) to increase the dataset to 14,000 images, with each class balanced at 2,000 images.
 - Image Preprocessing: All images were resized to 128x128 pixels and standardized for model input.
