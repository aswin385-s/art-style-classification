Project Description

Built an Art Style Classification system using a Convolutional Neural Network (CNN) trained on the ArtBench-10 dataset. The model classifies paintings into different artistic styles by learning visual features such as color patterns, textures, shapes, and brushstroke characteristics. Images are resized and normalized before training, and the model is evaluated using training/validation accuracy and loss.

CNN Architecture
Input Image (128 × 128 × 3)
        ↓
Conv2D - 32 filters, 3×3, ReLU
        ↓
MaxPooling2D - 2×2
        ↓
Conv2D - 64 filters, 3×3, ReLU
        ↓
MaxPooling2D - 2×2
        ↓
Conv2D - 128 filters, 3×3, ReLU
        ↓
MaxPooling2D - 2×2
        ↓
Flatten
        ↓
Dense - 128 neurons, ReLU
        ↓
Dropout - 0.3
        ↓
Dense - 10 neurons, Softmax
        ↓
Predicted Art Style

The convolution layers extract visual features, max-pooling layers reduce spatial dimensions, the dense layer performs classification, and Softmax produces probabilities for the 10 ArtBench-10 art-style classes.
