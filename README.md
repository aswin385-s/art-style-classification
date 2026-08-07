# Art Style Classification Using CNN

A Convolutional Neural Network (CNN)-based image classification system developed using Python and TensorFlow/Keras to automatically classify paintings into different artistic styles.

The project uses the ArtBench-10 dataset and learns visual characteristics such as colors, textures, shapes, patterns, and brushstroke features from artwork images.

## Features

* CNN-based art style classification
* ArtBench-10 dataset
* 10 different art style classes
* Image resizing to 128x128
* Image normalization
* Automatic visual feature extraction
* Convolution and max-pooling layers
* Dropout for reducing overfitting
* Softmax-based multi-class classification
* Training and validation performance monitoring
* Accuracy and loss visualization
* Prediction on unseen artwork images
* Google Colab compatible

## Architecture

```text
Input Artwork (128x128x3)
        ↓
Conv2D (32 Filters, 3x3, ReLU)
        ↓
MaxPooling2D (2x2)
        ↓
Conv2D (64 Filters, 3x3, ReLU)
        ↓
MaxPooling2D (2x2)
        ↓
Conv2D (128 Filters, 3x3, ReLU)
        ↓
MaxPooling2D (2x2)
        ↓
Flatten
        ↓
Dense (128, ReLU)
        ↓
Dropout (0.3)
        ↓
Dense (10, Softmax)
        ↓
Predicted Art Style
```

## Technologies

* Python
* TensorFlow / Keras
* Convolutional Neural Network (CNN)
* NumPy
* Matplotlib
* ArtBench-10
* Google Colab
