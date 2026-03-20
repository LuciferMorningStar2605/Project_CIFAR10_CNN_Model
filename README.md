# CIFAR-10 CNN Model

Deep learning image classification project for CIFAR-10 using a custom CNN trained in TensorFlow/Keras.

## Overview
This notebook implements a complete CNN pipeline for classifying CIFAR-10 images into ten object categories. It includes preprocessing, normalization, label encoding, visualization, training, and post-training evaluation with a confusion matrix.

## Tech Stack
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn

## Workflow
1. Load CIFAR-10 from Keras datasets
2. Inspect the data and verify preprocessing quality
3. Normalize pixel intensities and encode labels
4. Train a multi-layer CNN with convolution, pooling, and dropout
5. Track learning curves for loss and accuracy
6. Evaluate the model on the held-out test set
7. Visualize prediction behavior with a confusion matrix

## Model Notes
- Optimizer: `RMSprop`
- Loss: `categorical_crossentropy`
- Architecture: stacked `Conv2D` blocks followed by dense classification layers
- Regularization: dropout in convolutional and classifier stages

## Result
Notebook output shows test accuracy of roughly `79%`, indicating a stronger CIFAR-10 baseline than the simpler CNN variant.

## Files
```text
Project_CIFAR10_CNN_Model/
├── project_CIFAR10.ipynb
├── requirements.txt
└── README.md
```

## Run Locally
```bash
pip install -r requirements.txt
jupyter notebook project_CIFAR10.ipynb
```

## Learning Focus
- Building CNN baselines for color image classification
- Monitoring training vs validation behavior
- Improving performance through optimizer and architecture choices
- Error analysis with confusion matrices
