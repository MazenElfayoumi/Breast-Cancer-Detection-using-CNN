# Breast Cancer Detection using CNN

## Overview
This project applies Convolutional Neural Networks (CNNs) for the detection of Invasive Ductal Carcinoma (IDC) in breast cancer histopathological images. The model utilizes various CNN architectures to classify image patches as IDC-positive or IDC-negative.

## Dataset
- **Images**: 4500 normal, 3000 IDC-positive patches
- **Size**: 150x150 pixels

## CNN Architecture
- **Input Layer**: Accepts images of shape 150x150x3
- **Initial Convolutional Layer**: 64 filters, 3x3 size, ELU activation
- **Residual Blocks**: 
  - 1st Block: 64 filters
  - 2nd Block: 128 filters
  - 3rd Block: 256 filters, followed by global average pooling
- **Output Layer**: Dense layer with sigmoid activation

## Training
- **Optimizer**: RMSprop
- **Loss Function**: Binary cross-entropy
- **Early Stopping**: Enabled
- **Learning Rate Adjustment**: Applied

## Evaluation
- **Metrics**: Accuracy, Precision, Recall, ROC Curve
- **Cross-Validation**: 5-fold
