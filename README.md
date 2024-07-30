
# Image Segmentation with U-Net

This notebook demonstrates how to perform image segmentation using a U-Net model. The process includes loading and preprocessing the data, building the model, training, evaluation, and visualization of the results.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Data Loading and Preprocessing](#data-loading-and-preprocessing)
- [Model Building](#model-building)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Visualization](#visualization)

## Introduction

Image segmentation is the task of partitioning an image into multiple segments or regions, often used to identify and isolate regions of interest. U-Net is a popular deep learning model for this task, especially in biomedical image segmentation.
# Dataset Info
The dataset model is trained on contains a large number of segmented nuclei images.
## Prerequisites

- Python 3.x
- TensorFlow
- NumPy
- Matplotlib
- scikit-learn

## Data Loading and Preprocessing

The `load_data` function is used to load and preprocess the images and masks. The images and masks are resized to the specified dimensions.

## Model Building

The `build_unet_model` function builds a U-Net model with down-sampling, bottleneck, and up-sampling layers. The model is compiled with the Adam optimizer and binary cross-entropy loss.

## Model Training

The data is split into training and validation sets. Data augmentation is applied, and the model is trained using the augmented data.

## Evaluation

The model is evaluated on the validation set.

## Visualization

Random samples from the validation set are visualized, including the input image, ground truth mask, and predicted mask.

