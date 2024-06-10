# Handwritten Digits Classifier with PyTorch

This repository contains a project that implements a handwritten digits classifier using the PyTorch library. The classifier is trained on the MNIST dataset, which consists of 60,000 training images and 10,000 testing images of handwritten digits (0-9). The goal of this project is to achieve a high accuracy in recognizing these digits.

## Project Overview

The project follows these steps:

1. **Data Preprocessing**:
    - Transforms are applied to convert images to tensor form and normalize them from 0 to 1.
    - Further normalization is done with a standard value of mean and std = 0.5.
    - The MNIST dataset is downloaded and loaded.
    - DataLoaders are initialized with batch sizes, and the training data is split into training and validation sets for use during the training phase.

2. **Exploratory Data Analysis**:
    - The dataset is visualized, and its dimensions are checked.
    - Detailed information about the dataset is gathered to understand its structure.

3. **Neural Network Architecture**:
    - A simple feedforward neural network is defined.
    - The loss function (Cross-Entropy Loss) and optimizer (Adam) are initialized.

4. **Training Process**:
    - The model is trained, and the training loss and validation loss are plotted to monitor the training process.

5. **Model Evaluation**:
    - The trained model is tested on the test dataset, achieving an accuracy of 97%.

6. **Model Improvements**:
    - The exact mean and std of the dataset are calculated and used for normalization.
    - The architecture of the network is modified, and features like dropout are used to avoid overfitting.
    - The optimizer is changed to SGD optimizer.
    - The improved model is trained and tested, achieving an accuracy around 97%.
    - The final accuracy does not increase significantly because the initial accuracy was already very high.

7. **Model Saving**:
    - The trained model is saved using `torch.save` for future use.

## Getting Started

### Prerequisites

- Python 3.6+
- PyTorch
- torchvision
- NumPy
- Matplotlib

### Installing Dependencies

You can install the required dependencies using `pip`:

```bash
pip install torch torchvision numpy matplotlib
