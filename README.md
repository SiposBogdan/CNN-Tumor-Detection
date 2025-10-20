# 🧠 Brain Tumor Detection using CNN

This repository contains a Jupyter Notebook (`sample.ipynb`) that demonstrates how to automatically classify MRI brain images as **Tumor** or **No Tumor** using a **Convolutional Neural Network (CNN)**.  
The project aims to support early detection and diagnosis of brain tumors through deep learning techniques applied to medical imaging.

---

## 🩺 Project Overview

Brain tumor detection is a critical task in medical imaging that directly influences patient prognosis and treatment planning.  
Using MRI scans from the **Brain Tumor Multimodal Image (CT & MRI)** dataset, this project builds a **binary image classifier** that distinguishes between:

- **Tumor:** Glioma, Meningioma, and Pituitary tumor images  
- **No Tumor:** Healthy MRI scans  

---

## ⚙️ Workflow

### 1. Data Preparation
- Curates and relabels MRI images into binary categories  
- Applies preprocessing steps:
  - Image resizing and normalization  
  - Data augmentation (rotation, flip, zoom) to improve generalization  

### 2. Model Architecture
- Custom **Sequential CNN model** with:
  - Convolution + MaxPooling layers  
  - Batch Normalization & Dropout for regularization  
  - Fully connected dense layers for final classification  
- Implemented using **TensorFlow / Keras**

### 3. Training
- Compiles model with `binary_crossentropy` loss and `adam` optimizer  
- Evaluates performance using **accuracy**, **precision**, **recall**, and **F1-score**  
- Visualizes learning curves (training vs validation accuracy/loss)

### 4. Evaluation & Results
- Displays **confusion matrix** and **classification report**  
- Visualizes predictions on test samples  
- Achieves **high accuracy** in distinguishing tumor vs. non-tumor MRI images  

---

## 🧮 Example Results

| Metric | Result | Description |
|--------|---------|-------------|
| **Training Accuracy** | ~98% | Model performance on training data |
| **Validation Accuracy** | ~96% | Indicates good generalization |
| **Test Accuracy** | ~95–97% | Robust on unseen data |
| **Precision** | >95% | Reliable positive tumor detection |
| **Recall** | >93% | Strong sensitivity for tumor detection |
| **ROC–AUC** | >0.97 | Excellent class separability |

**Visualization Outputs:**
- Accuracy and loss curves  
- Confusion matrix  
- Predicted MRI samples with tumor classification  

---
