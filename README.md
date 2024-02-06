# Convolutional Neural Network (CNN) Model

This repository contains the configuration and weights for a Convolutional Neural Network (CNN) model trained on image data. The model architecture is defined using the Keras Sequential API.

## Model Architecture

The model is defined as a Sequential model with the following layers:

1. Input Layer
Input shape: (None, 32, 32, 1)

2. Convolutional Layer
Filters: 32
Kernel size: (3, 3)
Activation function: ReLU
Batch normalization
Max pooling: pool size (2, 2), strides (2, 2)

3. Dropout Layer
Dropout rate: 0.25

4. Convolutional Layer
Filters: 64
Kernel size: (3, 3)
Activation function: ReLU
Batch normalization
Max pooling: pool size (2, 2), strides (2, 2)

5. Dropout Layer
Dropout rate: 0.25
Flatten Layer

6. Dense Layer
Units: 128
Activation function: ReLU
Batch normalization

7. Dropout Layer
Dropout rate: 0.5

8. Dense Layer
Units: 6 (output layer)
Activation function: Softmax

## Categories to Predict

The model predicts images into the following categories:
- Accessories
- Bags
- Clothes
- Shoes
- Watches


## Model Files

- `model_config.json`: Configuration file containing the model architecture.
- `model_weights.h5`: File containing the model weights.


Feel free to use this model for your category classification tasks!