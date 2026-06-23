# AI-Generated Image Classification using Deep Learning

This repository contains the implementation of a binary image classification system for distinguishing between AI-generated and real human images. The project uses transfer learning-based deep learning models, particularly MobileNetV2 and ResNet50, to evaluate their effectiveness in AI-generated image detection.

## 📌 Project Overview

The rapid development of generative artificial intelligence has increased the need for reliable detection systems that can identify AI-generated visual content. This project focuses on classifying images into two categories:

- **AI-generated images**
- **Real human images**

The implementation was developed using TensorFlow/Keras and evaluated on the DeepDetect-2025 dataset.

## 🧠 Models Used

This repository includes experiments using the following deep learning architectures:

| Model | Description |
|---|---|
| MobileNetV2 | Lightweight convolutional neural network using transfer learning with ImageNet pretrained weights |
| ResNet50 | Residual neural network architecture used as a comparative model |

## 🗂️ Dataset

The dataset used in this project is the **DeepDetect-2025** dataset, publicly available on Kaggle.

Dataset source:  
https://www.kaggle.com/datasets/ayushmandatta1/deepdetect-2025

The dataset consists of image samples categorized into AI-generated and real human classes.

## ⚙️ Training Configuration

The main training configuration used in this project is summarized below:

| Parameter | Value |
|---|---|
| Task | Binary image classification |
| Input size | 224 × 224 × 3 for MobileNetV2 |
| Optimizer | Adam |
| Learning rate | 0.001 |
| Batch size | 32 |
| Epochs | 15 |
| Loss function | Binary Crossentropy |
| Pretrained weights | ImageNet |
| Framework | TensorFlow/Keras |

## 📁 Repository Structure

```text
.
├── README.md
├── requirements.txt
├── notebooks/
│   ├── mobilenetv2.ipynb
│   └── resnet50.ipynb
├── src/
│   ├── train_mobilenetv2.py
│   ├── train_resnet50.py
│   └── evaluate.py
├── docs/
│   └── figures/
└── results/
