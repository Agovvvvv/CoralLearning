# Coral Classification using Supervised Methods

## Overview 

This project aims to classify coral images using both supervised and unsupervised machine learning methods. The goal is to compare the performance of these two approaches in identifying coral characteristics from images. 🐠

## Introduction 

Corals are vital to marine biodiversity and the overall health of our oceans. An automated system for classifying corals can significantly speed up the work of ocean specialists. This project explores an unsupervised model, which has the potential to eliminate the time-consuming process of manually labeling each coral image.

## Methodology 

The project follows these key steps:

1.  **Feature Extraction**: Images are first converted from RGB to grayscale. Then, texture features are extracted using the **Gray-Level Co-occurrence Matrix (GLCM)** and **Local Binary Patterns (LBP)** algorithms. These features are then stored in a DataFrame for analysis.

2.  **Visualization**: To better understand the data, **Principal Component Analysis (PCA)** is used to visualize the extracted features in a 3D space.

3.  **Supervised Classification**:
    * The dataset is split into training and testing sets.
    * A **Logistic Regression** model is trained to classify the corals.
    * The model's performance is evaluated using metrics like **accuracy**, a **confusion matrix**, and a **classification report**.

4.  **Comparison**: Finally, the accuracies of the Logistic Regression and K-Means models are compared to determine the more effective approach for this classification task.

## 🚀 Getting Started 

### Prerequisites

Make sure you have Python installed on your system. You will also need to install the following libraries:

```bash
pip install opencv-python matplotlib numpy pandas seaborn scikit-image mahotas scikit-learn tqdm
