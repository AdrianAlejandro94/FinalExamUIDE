# TensorFlow CNN Model

This repository contains a Convolutional Neural Network (CNN) model implemented using TensorFlow. The model is trained to classify images into two classes using a dataset.

## Installation

To run this project, you need to have the following dependencies installed:

- TensorFlow
- PIL
- NumPy

You can install the dependencies using the following command:

```
pip install tensorflow pillow numpy
```

## Dataset

The dataset used for training and testing the model is located in the following directory:

```
C:\Users\aarte\OneDrive\Desktop\ExamenTratamientoDatos\dataset
```

The dataset directory should have the following structure:

```
dataset
├── train
│   ├── class1
│   ├── class2
│   └── ...
└── test
    ├── class1
    ├── class2
    └── ...
```

Please make sure to organize your dataset accordingly.

## Model Architecture

The CNN model architecture consists of the following layers:

1. Convolutional layer with 32 filters and ReLU activation
2. Convolutional layer with 64 filters and ReLU activation
3. MaxPooling layer with a pool size of 2x2
4. Dropout layer with a rate of 0.25
5. Flatten layer
6. Dense layer with 128 units and ReLU activation
7. Dropout layer with a rate of 0.5
8. Dense layer with 1 unit and sigmoid activation

The model is compiled with the Adam optimizer and binary cross-entropy loss function.

## Training

The training process involves the following steps:

1. Image pre-processing and data augmentation
2. Generating batches of training, validation, and testing data
3. Training the model for a specified number of epochs

The model is trained for 10 epochs using the training and validation data.

## Saving the Model

After training, the model is saved as `modelo_CNN.h5` in the following directory:

```
C:\Users\aarte\OneDrive\Desktop\ExamenTratamientoDatos\
```

## Usage

You can use this model for image classification tasks by loading the saved model and making predictions on new images.
