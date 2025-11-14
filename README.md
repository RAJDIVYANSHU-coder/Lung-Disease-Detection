#  Lung Disease Detection Using Deep Learning

## Project Overview
This project focuses on detecting different types of lung diseases using deep learning methods.  
A convolutional neural network (CNN) based on **MobileNetV2** is trained on chest X-ray images to classify lung conditions.  
The goal of the project is to assist in early and accurate identification of diseases using automated image analysis.

---

##  Dataset
Due to size limitations, the dataset used for training and testing is stored in Google Drive.

**Download Dataset:**  
[Dataset Link](https://drive.google.com/drive/folders/1oSQTN70B4pEEb6Xxl9tNgOdeRIGdG-0r?usp=drive_link)

The dataset consists of multiple lung disease classes such as:
- COVID-19  
- Normal  
- Bacterial Pneumonia  
- Viral Pneumonia  

---

## Files Included in This Repository
This GitHub repository includes the following files:

- **`Lung_Disease_Detection.ipynb`** — Jupyter Notebook containing the full model training pipeline  
- **`Lung_Disease_Detection.pptx`** — Project presentation  
- **`Lab_Report.pdf`** — Complete project report  
- Additional supporting code or visualizations (if any)

The dataset is NOT uploaded here due to size, but accessible via the provided Drive link.

---

## Model Architecture & Workflow

### **1. Data Preprocessing**
- Image resizing to **128×128**
- Scaling pixel values
- Train-test split
- Image augmentation using:
  - rotation
  - zoom
  - horizontal flip
  - width/height shift

### **2. Transfer Learning Model**
The model is built using:
- **MobileNetV2** as the base model (pretrained on ImageNet)
- Global Average Pooling layer
- Dense layers with Dropout regularization
- Softmax output layer for multi-class classification

### **3. Training Details**
- Loss function: `categorical_crossentropy`
- Optimizer: `adam`
- Metrics: `accuracy`
- Regularization: `Dropout`, `L2`
- EarlyStopping callback to prevent overfitting

---

## Evaluation Metrics

The model is evaluated using:

- **Accuracy score**
- **Classification report**
- **Confusion matrix**
- **Loss and accuracy curves**

These diagnostics help in analyzing model performance and identifying misclassifications.

---
