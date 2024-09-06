# Plant Disease Detection using ResNet50

This project uses a pre-trained ResNet50 deep learning model for detecting plant diseases. The model is fine-tuned for binary classification to identify healthy and diseased plant images.

## Project Overview

Plant disease detection is a crucial application in agriculture. The goal of this project is to develop an image classification model that can distinguish between healthy and diseased plants using a dataset of plant images. The project is implemented using TensorFlow and Keras.

## Dataset

The dataset used for this project contains images of healthy and diseased plants. The dataset is divided into training and validation sets, and data augmentation is applied to enhance the performance of the model.

- **Training Images:** 329 images
- **Validation Images:** 81 images
- **Classes:** Healthy, Diseased

## Model Architecture

The project uses the ResNet50 architecture, which is a convolutional neural network (CNN) pre-trained on the ImageNet dataset. ResNet50's convolutional base is frozen, and custom dense layers are added on top to adapt it to our binary classification problem.

### Layers Added:

- Flatten layer
- Dense layer with 512 units and ReLU activation
- Dropout layer with 50% probability
- Output layer with a single unit and sigmoid activation for binary classification

### Optimizer

- **Adam optimizer** with a learning rate of 0.001
- **Loss function:** Binary crossentropy
