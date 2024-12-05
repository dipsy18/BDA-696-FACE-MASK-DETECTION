# Face Mask Detection - BDA-696 Final Group Project

## Group Members:
- Dhrumil Buch
- Sharad Parmar
- Jani Miya Shaik
- Dipsy
- Aditya Desale

## Abstract
This project develops a deep learning-based face mask detection system designed for real-time monitoring of mask compliance, an essential public health measure during the COVID-19 pandemic. Using a dataset of over 7,500 images categorized by mask status, the system classifies individuals as either wearing or not wearing a face mask. Several deep learning models, including CNN, MobileNet, VGG16, ResNet, YOLO, and SSD, were evaluated for accuracy and real-time performance.

## Introduction
The COVID-19 pandemic highlighted the importance of monitoring mask-wearing compliance. This project aims to build an efficient face mask detection model suitable for deployment in various real-time surveillance systems, contributing to public health safety by ensuring mask-wearing compliance.

## Problem Statement
The primary goal of this project is to develop a reliable and efficient model capable of detecting face masks in real-time. The model should operate effectively in diverse environments and support public health policies related to mask-wearing during pandemics.

## Dataset Description
The dataset contains 7,553 images of individuals, categorized into:
- 3,725 images of individuals wearing masks
- 3,828 images of individuals not wearing masks

The images are in RGB format, and the total dataset size is 171 MB. The dataset is organized into two labeled folders: 'with_mask' and 'without_mask'. The dataset is sourced from Prajna Bhandary’s GitHub repository and supplemented with additional images from Google search results.

## Methodology
1. **Data Acquisition**: The dataset is split into two categories, mask-wearing and non-mask-wearing individuals.
2. **Data Preprocessing**: Images are resized to 224x224 pixels and normalized to a [0,1] scale. Data augmentation techniques such as rotation, flipping, and scaling are applied.
3. **Model Development**:
   - Baseline CNN model for initial evaluation.
   - Fine-tuning of pre-trained models like MobileNetV2, VGG16, and ResNet50.
   - Real-time detection models like YOLO and SSD for live video streams.
4. **Model Training**: Models are trained using the Adam optimizer with categorical cross-entropy loss.
5. **Model Evaluation**: Models are evaluated using metrics like accuracy, precision, recall, F1-score, and confusion matrix.
