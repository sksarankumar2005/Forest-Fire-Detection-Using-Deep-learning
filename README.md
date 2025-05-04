# 🌲 Forest Fire Detection using Deep Learning 🔥
## WEEK 3
## 🎯 Objective
The goal of this project is to build a deep learning model that can accurately detect forest fires from images. This solution aims to support real-time wildfire monitoring and contribute to disaster prevention efforts.

---

## 🧰 Technologies Used
- **Programming Language:** Python  
- **Framework:** TensorFlow / Keras  
- **Libraries:** NumPy, Matplotlib, OpenCV, PIL, Streamlit  
- **Dataset:** Wildfire Dataset from Kaggle  
- **Deployment Tool:** Streamlit  

---

## 🚀 Project Overview

### 📥 Data Acquisition and Setup
- Downloaded the Wildfire Dataset using the Kaggle API.  
- Organized image data into separate folders for `fire` and `no_fire` classes.  
- Loaded necessary libraries and checked for GPU support to optimize training.

### 🔍 Data Exploration and Preprocessing
- Visualized sample images to understand the dataset.  
- Checked class distribution and image shapes for consistency.  
- Used `ImageDataGenerator` to normalize pixel values and create train/validation/test sets.  
- Mapped class indices to readable labels.

### 🏗️ Model Building
Designed a **Convolutional Neural Network (CNN)** using Keras' Sequential API:
- Conv2D and MaxPooling2D layers for feature extraction  
- Flatten and Dense layers for classification.  
- Dropout layer to reduce overfitting. 
- Output layer with sigmoid activation for binary classification.  

### 🏋️ Model Training
- Compiled the model using the **Adam optimizer** and **binary cross-entropy** loss.  
- Trained the model while monitoring validation accuracy.  
- Used **EarlyStopping** and **ModelCheckpoint** to save the best weights.

### 📊 Model Evaluation
- Evaluated the model on the test dataset.  
- Assessed performance using accuracy, precision, recall, and F1-score.  
- Visualized results with a **confusion matrix**.

### 🔎 Predictions and Testing
- Ran predictions on unseen images to check generalization.  
- Compared model predictions with actual labels to validate accuracy.

### 🌐 Deployment
- Built a user-friendly **Streamlit web app** for real-time fire detection.  
- Allowed users to upload images and receive instant predictions.  
- Displayed class label and prediction confidence score.

---

## ✅ Final Outcome
The model successfully classifies images as **fire** or **no fire** with high accuracy.  
The web app makes the solution accessible for real-time wildfire monitoring and decision-making.
