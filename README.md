# AI Image Processing Project

## Overview

This project focuses on classifying images using a Convolutional Neural Network (CNN) implemented with TensorFlow and Keras. The model is trained to categorize images into three distinct classes.

## Dataset

The dataset comprises images organized into three categories. The data is split into training, validation, and test sets using the `splitfolders` library:

- **Training Set**: 80% of the data
- **Validation Set**: 10% of the data
- **Test Set**: 10% of the data

## Model Architecture

The CNN model consists of the following layers:

1. **Convolutional Layer**: 32 filters of size 3x3, activation function ReLU
2. **MaxPooling Layer**: Pool size of 2x2
3. **Convolutional Layer**: 64 filters of size 3x3, activation function ReLU
4. **MaxPooling Layer**: Pool size of 2x2
5. **Flatten Layer**: Converts 2D matrices to a 1D vector
6. **Dense Layer**: 128 neurons, activation function ReLU
7. **Dropout Layer**: Dropout rate of 0.5 to prevent overfitting
8. **Dense Output Layer**: 3 neurons (corresponding to the three classes), activation function Softmax

The model is compiled with the Adam optimizer and categorical cross-entropy loss function.

## Installation

To set up the project environment, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/nikhil-1111/AI-Image-processing-project.git
