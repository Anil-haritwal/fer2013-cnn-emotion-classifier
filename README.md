# Facial Emotion Recognition using CNN (FER2013)
👨‍💻 Author: Anil Haritwal

## Project Overview
This project implements a **Convolutional Neural Network (CNN)** from scratch to classify **facial emotions** using the **FER2013 dataset**. The model predicts 7 emotion classes:  
**Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral**.

The goal is to demonstrate **deep learning fundamentals**, CNN design, and image classification workflows.

---

## Dataset
- **Name:** FER2013  
- **Source:** [Kaggle FER2013 Dataset](https://www.kaggle.com/msambare/fer2013)  
- **Image Size:** 48×48 pixels  
- **Channels:** Grayscale (1 channel)  
- **Classes:** 7  

---

## Features & Highlights
- Built a **CNN from scratch** with multiple Conv2D, MaxPooling2D, BatchNormalization, Dropout, and Dense layers.  
- Applied **data augmentation** for better generalization.  
- Evaluated the model on test data with metrics like **accuracy and loss**.  
- Fully implemented in **TensorFlow/Keras**.

---

## Model Architecture
```text
Input: 48x48x1 grayscale images
↓
Conv2D + ReLU + MaxPooling + BatchNorm + Dropout
↓
Conv2D + ReLU + MaxPooling + BatchNorm + Dropout
↓
Conv2D + ReLU + MaxPooling + BatchNorm + Dropout
↓
Flatten
↓
Dense (256) + ReLU + Dropout
↓
Dense (128) + ReLU + Dropout
↓
Dense (64) + ReLU
↓
Dense (7) + Softmax
Output: 7 emotion probabilities
