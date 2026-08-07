Art Style Classification using CNN

Built an Art Style Classification system using a Convolutional Neural Network (CNN) trained on the ArtBench-10 dataset to classify paintings into 5 different artistic styles. Images are resized to 128×128 and normalized before being passed through the CNN. The model learns visual features such as colors, textures, shapes, patterns, and brushstroke characteristics to identify the corresponding art style.

CNN Architecture:
Input Image (128×128×3)
→ Conv2D (32 filters, 3×3, ReLU)
→ MaxPooling2D (2×2)
→ Conv2D (64 filters, 3×3, ReLU)
→ MaxPooling2D (2×2)
→ Conv2D (128 filters, 3×3, ReLU)
→ MaxPooling2D (2×2)
→ Flatten
→ Dense (128, ReLU)
→ Dropout (0.3)
→ Dense (10, Softmax)
→ Predicted Art Style

Technologies: Python, TensorFlow/Keras, CNN, NumPy, Matplotlib, ArtBench-10
