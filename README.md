# 🖼️ CIFAR-10 Image Classification with CNN

This project implements a **Convolutional Neural Network (CNN)** to classify images from the **CIFAR-10 dataset** into 10 categories.  
The CIFAR-10 dataset is a benchmark in machine learning and computer vision, containing tiny color images in 10 different classes.  
This project demonstrates how deep learning models can achieve high accuracy in multi-class image classification.

---

## 📌 Project Overview

- Dataset: **CIFAR-10** (60,000 images: 50,000 training, 10,000 test)  
- Classes: `airplane`, `automobile`, `bird`, `cat`, `deer`, `dog`, `frog`, `horse`, `ship`, `truck`  
- Model: **Custom CNN** built using **TensorFlow/Keras**  
- Key Features:
  - Data preprocessing & normalization
  - CNN architecture with Conv2D, MaxPooling, Dropout, Dense layers
  - Training, validation, and testing
  - Performance evaluation with accuracy, loss curves, and confusion matrix  

---

## 📂 Dataset

- **Source**: [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) (also available via `keras.datasets`)  
- **Images**: 32x32 color images  
- **Preprocessing**:
  - Normalized pixel values (0–1 range)  
  - One-hot encoded labels  

---

## ⚙️ Methodology & Workflow

1. **Data Loading**
   - Loaded CIFAR-10 dataset from `keras.datasets`  

2. **Preprocessing**
   - Normalized pixel values  
   - Encoded labels into categorical format  

3. **Model Architecture**
   - **Convolutional layers** (feature extraction)  
   - **MaxPooling layers** (dimensionality reduction)  
   - **Dropout** (regularization)  
   - **Fully connected layers** (classification)  
   - Output: 10 neurons with `softmax` activation  

4. **Training**
   - Optimizer: `Adam`  
   - Loss: `categorical_crossentropy`  
   - Metric: `accuracy`  

5. **Evaluation**
   - Plotted training vs validation accuracy/loss  
   - Generated confusion matrix and classification report  

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Deep Learning**: `tensorflow`, `keras`
- **Data Handling**: `numpy`, `pandas`
- **Visualization**: `matplotlib`, `seaborn`
- **Metrics**: `scikit-learn`

---

## 🚀 Installation

Clone this repository:

```bash
git clone https://github.com/yourusername/cifar10-image-classification.git
cd cifar10-image-classification
