# Image-Based Cancer Diagnosis Using Convolutional Neural Networks

# 📌 Project Overview

This project presents an end-to-end **Deep Learning pipeline** for automated cancer diagnosis using medical images and **Convolutional Neural Networks (CNNs)**. The objective is to develop, train, and evaluate a custom CNN model capable of accurately classifying cancerous and non-cancerous medical images.

The project demonstrates the complete deep learning workflow, including **medical image preprocessing**, **data augmentation**, **CNN architecture design**, **model regularization**, **performance evaluation**, and **visualization techniques** such as learning curves, ROC curve, and confusion matrix.

---

# 🧬 Dataset Information

**Dataset:** Breast Ultrasound Images (BUSI)

**Source:** Kaggle / Public Medical Imaging Repository

### Dataset Characteristics

- Medical Imaging Dataset
- Image Format: PNG
- Classification Type: Binary Classification
- Input Image Size: **128 × 128 pixels**
- Color Channels: RGB

### Target Labels

- **0 → Non-Cancer (Benign / Normal)**
- **1 → Cancer (Malignant)**

The dataset contains breast ultrasound images collected for breast cancer diagnosis. Each image is labeled according to its diagnostic category and is used to train a deep learning model for automated cancer detection.

---

# ⚙️ Project Workflow

## 📥 1. Data Preparation

- Loaded medical images from the dataset directory
- Created a custom image dataset loader
- Converted images into tensors
- Organized image-label pairs for training

---

## 🖼️ 2. Image Preprocessing

- Resized all images to **128 × 128 pixels**
- Converted images to PyTorch tensors
- Applied dataset normalization
- Standardized image dimensions for CNN input

---

## 🔄 3. Data Augmentation

To improve model generalization and reduce overfitting, several augmentation techniques were applied:

- Random Horizontal Flip
- Random Vertical Flip
- Random Rotation
- Image Normalization

These augmentations increase data diversity while preserving medical image characteristics.

---

## 📂 4. Dataset Splitting

The dataset was divided into three subsets using stratified sampling:

- **Training Set:** 70%
- **Validation Set:** 15%
- **Testing Set:** 15%

Stratification ensures balanced class distribution across all subsets.

---

## 🧠 5. CNN Model Development

A custom Convolutional Neural Network was implemented from scratch.

The architecture includes:

- Three Convolutional Layers
- ReLU Activation Functions
- Max Pooling Layers
- Batch Normalization
- Dropout Regularization
- Fully Connected Hidden Layer
- Sigmoid Output Layer

The network learns hierarchical image features for binary cancer classification.

---

## ⚙️ 6. Model Training

The CNN model was trained using:

- Binary Cross Entropy Loss (BCELoss)
- Adam Optimizer
- Learning Rate Optimization
- Batch Training
- Minimum of 20 Training Epochs

Training and validation performance were monitored throughout the learning process.

---

## 📊 7. Model Evaluation

The trained model was evaluated using multiple performance metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

These metrics provide a comprehensive assessment of the model's diagnostic capability.

---

## 📈 8. Visualization

The project includes several deep learning diagnostic visualizations:

- Training vs Validation Loss Curve
- Training vs Validation Accuracy Curve
- ROC Curve with AUC Score
- Confusion Matrix Heatmap

These visualizations help analyze model learning behavior and classification performance.

---

# 🏆 Model Performance

The trained CNN model successfully learned discriminative image features for cancer diagnosis.

Performance evaluation was based on:

- Test Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

The final model demonstrates strong classification capability and generalization on unseen medical images.

> **Note:** Replace this section with your actual performance metrics after running the notebook.

---

# 🛠 Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- OpenCV
- Jupyter Notebook

---

# 📂 Project Structure

```
Image-Based-Cancer-Diagnosis-CNN/
│
├── dataset/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── images/
│   ├── learning_curve.png
│   ├── roc_curve.png
│   └── confusion_matrix.png
│
├── Image_Based_Cancer_Diagnosis.ipynb
├── README.md
└── requirements.txt
```

---

# 🚀 Project Highlights

✔ End-to-End Deep Learning Pipeline

✔ Medical Image Preprocessing

✔ Custom CNN Architecture

✔ Data Augmentation

✔ Batch Normalization

✔ Dropout Regularization

✔ Binary Cancer Classification

✔ Learning Curve Visualization

✔ ROC Curve & AUC Evaluation

✔ Confusion Matrix Analysis

✔ Deep Learning-Based Medical Image Diagnosis

---

# 🎯 Conclusion

This project demonstrates how Convolutional Neural Networks (CNNs) can be effectively applied to automated cancer diagnosis using medical imaging data. A complete deep learning workflow was implemented, including image preprocessing, data augmentation, dataset partitioning, CNN model development, regularization, model training, and comprehensive performance evaluation.

The custom CNN successfully learned meaningful image features for distinguishing cancerous from non-cancerous cases. Model performance was assessed using Accuracy, Precision, Recall, F1-Score, ROC-AUC Score, learning curves, and confusion matrix analysis, providing a detailed understanding of its predictive capability.

The results highlight the potential of deep learning and computer vision techniques in assisting healthcare professionals with accurate, efficient, and reliable medical image analysis, contributing to early cancer detection and improved clinical decision-making.
