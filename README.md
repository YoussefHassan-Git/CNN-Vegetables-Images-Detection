# Vegetable Classification using CNN 🌿🥕🍅

This repository contains the implementation of a Convolutional Neural Network (CNN) model to classify images of 15 different vegetables. The model leverages deep learning to accurately predict the category of a given vegetable image from the provided dataset.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Data Preprocessing](#data-preprocessing)
- [Training and Evaluation](#training-and-evaluation)
- [Results](#results)
- [Graphs and Performance](#graphs-and-performance)

## Project Overview

This project is designed to classify 15 different types of vegetables using a CNN model. By applying deep learning techniques, the model identifies vegetables like **tomato**, **carrot**, **potato**, etc., from a collection of images with high accuracy.


## Dataset

The dataset used consists of 15 categories of vegetables:
1. Broccoli
2. Capsicum
3. Bottle Gourd
4. Radish
5. Tomato
6. Brinjal
7. Pumpkin
8. Carrot
9. Papaya
10. Cabbage
11. Bitter Gourd
12. Cauliflower
13. Bean
14. Cucumber
15. Potato

Each category contains multiple images for training, validation, and testing purposes. Here are a few sample images from the dataset:

![1528207b-d665-47b5-bc40-e1ac203b2b73](https://github.com/user-attachments/assets/bf2a3a49-2c78-47c9-8c87-4dcc656ea50e)


## Model Architecture

The model architecture is built using CNN layers to process the images. The architecture consists of:

- **Convolutional Layers**: Extracting features from input images
- **Max Pooling Layers**: Reducing dimensionality and computational load
- **Dropout Layers**: To avoid overfitting
- **Fully Connected Layers**: For classification into 15 categories
- **Softmax Activation**: For multi-class classification

## Data Preprocessing

Before feeding the images into the model:
- **Images are resized** to 150x150 pixels for uniformity.
- **Normalization**: Pixel values are scaled between 0 and 1.
- **Data Augmentation**: Random transformations like rotations, flips, and zooms are applied to increase the diversity of training samples.

## Training and Evaluation

The model was trained with:
- **Optimizer**: Adam
- **Loss Function**: Categorical Cross-Entropy
- **Metrics**: Accuracy, Loss, F1-Score
- **Training/Validation Split**: 80/20
- **Epochs**: 10


## Results

The model performed well on the validation dataset. Below are the overall results in terms of accuracy and F1-score for some classes.

| Vegetable        | Accuracy | F1-Score |
|------------------|----------|----------|
| Broccoli         | 96%      | 0.95     |
| Capsicum         | 94%      | 0.93     |
| Bottle Gourd     | 92%      | 0.91     |
| ...              | ...      | ...      |
| Potato           | 98%      | 0.97     |

## Graphs and Performance
--
Training, Validation Loss Graph:

![4dcfe631-b492-4760-817f-cb55c50d3855](https://github.com/user-attachments/assets/a403ebf7-6c09-4639-b2c9-42af40d8c319)

Training, Validation Accuracy Graph:

![45667fa5-5fac-4de5-91e6-3435711ad819](https://github.com/user-attachments/assets/59d3d81e-7ee0-4474-a4bf-47cef77ddea9)



