# CIFAR-10 Image Classifier (PyTorch)

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify images from the CIFAR-10 dataset.

## 📌 Features
- Implemented CNN from scratch with PyTorch
- Data augmentation (random crop, horizontal flip)
- Learning rate scheduler and dropout for regularization
- Achieved ~86% test accuracy

## 🚀 Tech Stack
- Python
- PyTorch
- Torchvision
- Matplotlib

## 📂 Files
- `cifar10_classifier.ipynb` → Colab notebook with full training code
- `requirements.txt` → Dependencies
- `README.md` → Project details

## 🔄 Loading the Model

To reuse the trained model later:

```python
import torch
from model import MyModelClass   # or redefine your CNN in the notebook

model = MyModelClass()
model.load_state_dict(torch.load('best_model.pth', map_location='cpu'))
model.eval()
