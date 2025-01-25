# Image-Classification
A simple three-class image classifier using neural networks CNN and ANN to classify images into Plants,Animals and Non-Living Things and to also compare the accuracy score differences between CNN and ANN.
## Introduction
The goal of this project is to classify images into one of four categories using both ANN and CNN models. The dataset consists of approximately 1278 images, with around 320 images per class. The images are preprocessed and augmented to improve model accuracy.

## Dataset
The dataset is divided into four classes:
- Animals
- Humans
- Plants
- Non-Living things

The images are collected from various sources, including manual collection and Google Images. The dataset is preprocessed to remove duplicates and ensure uniformity in size (32x32 pixels).

## Data Preprocessing
1. **Data Cleaning**: Duplicate images and images not in the required format are removed.
2. **Resizing and Renaming**: All images are converted to JPG format, renamed in order, and resized to 32x32 pixels.

## Data Augmentation
Data augmentation techniques, such as flipping (horizontal and vertical), are applied to increase the diversity of the training dataset.

## Model Architecture

### Artificial Neural Network (ANN)
The ANN model consists of the following layers:
- Input layer (Flattened input)
- Dense layer with 3000 neurons (ReLU activation)
- Dense layer with 1000 neurons (ReLU activation)
- Output layer with 10 neurons (Softmax activation)

### Convolutional Neural Network (CNN)
The CNN model consists of the following layers:
- Convolutional layer with 32 filters (3x3 kernel, ReLU activation)
- MaxPooling layer (2x2 pool size)
- Convolutional layer with 64 filters (3x3 kernel, ReLU activation)
- MaxPooling layer (2x2 pool size)
- Flatten layer
- Dense layer with 128 neurons (ReLU activation)
- Output layer with 10 neurons (Softmax activation)

## Training and Evaluation
Both models are trained using the preprocessed and augmented dataset. The dataset is split into training and testing sets (80% training, 20% testing). The models are evaluated based on their accuracy and loss on the test set.

### Results
- **ANN Test Accuracy**: ~66.96%
- **CNN Test Accuracy**: ~99.46%
