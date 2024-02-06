# Convolutional Neural Network (CNN) Model

This repository contains the configuration and weights for a Convolutional Neural Network (CNN) model trained on image data. The model architecture is defined using the Keras Sequential API.

## Model Architecture

The model is defined as a Sequential model with the following layers:

```json
{
    "class_name": "Sequential",
    "config": {
        "name": "sequential",
        "layers": [
            {
                "class_name": "InputLayer",
                "config": {
                    "batch_input_shape": [null, 32, 32, 1],
                    "dtype": "float32",
                    "sparse": false,
                    "ragged": false,
                    "name": "conv2d_input"
                }
            },
            {
                "class_name": "Conv2D",
                "config": {
                    "name": "conv2d",
                    "trainable": true,
                    "dtype": "float32",
                    "batch_input_shape": [null, 32, 32, 1],
                    "filters": 32,
                    "kernel_size": [3, 3],
                    "strides": [1, 1],
                    "padding": "valid",
                    "data_format": "channels_last",
                    "dilation_rate": [1, 1],
                    "groups": 1,
                    "activation": "relu",
                    "use_bias": true,
                    "kernel_initializer": {
                        "class_name": "GlorotUniform",
                        "config": {"seed": null}
                    },
                    "bias_initializer": {
                        "class_name": "Zeros",
                        "config": {}
                    },
                    "kernel_regularizer": null,
                    "bias_regularizer": null,
                    "activity_regularizer": null,
                    "kernel_constraint": null,
                    "bias_constraint": null
                }
            },
            // More layers ...
        ]
    },
    "keras_version": "2.12.0",
    "backend": "tensorflow"
}
```

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