#Forest Fire Detection using Deep Learning 🔥
#Objective
The goal of this project is to build a deep learning model that can accurately detect forest fires from images. This solution aims to support real-time wildfire monitoring and contribute to disaster prevention efforts.

#Technologies Used
Programming Language: Python

Framework: TensorFlow / Keras

Libraries: NumPy, Matplotlib, OpenCV, PIL, Streamlit

Dataset: Wildfire Dataset from Kaggle

Deployment Tool: Streamlit

##Project Overview
#Data Acquisition and Setup
Downloaded the Wildfire Dataset using the Kaggle API.

Organized image data into separate folders for fire and no_fire classes.

Loaded all necessary libraries and checked for GPU support to optimize model training.

#Data Exploration and Preprocessing
Visualized sample images to understand the dataset.

Checked class distribution and image shapes for consistency.

Applied preprocessing using ImageDataGenerator to normalize pixel values and split the data into training, validation, and test sets.

Mapped class indices to readable labels.

#Model Building
Designed a Convolutional Neural Network (CNN) using Keras' Sequential API:

Multiple Conv2D and MaxPooling2D layers for feature extraction.

Flatten and Dense layers for classification.

Dropout layer to prevent overfitting.

Final output layer with sigmoid activation for binary classification.

#Model Training
Compiled the model using the Adam optimizer and binary cross-entropy loss.

Trained the model with validation monitoring.

Implemented EarlyStopping and ModelCheckpoint to save the best weights during training.

#Model Evaluation
Evaluated the trained model on the test dataset.

Measured performance using accuracy, precision, recall, and F1-score.

Visualized results using a confusion matrix to analyze predictions.

#Predictions and Testing
Ran predictions on new/unseen images to test the model's generalization.

Compared predicted labels with actual labels for accuracy validation.

#Deployment
Built a clean and interactive Streamlit web app for real-time forest fire detection.

Users can upload an image, and the model predicts whether there’s a fire or no fire.

Displayed confidence scores along with predictions.

#Final Outcome
The model successfully classifies images as fire or no fire with high accuracy. The deployed app makes it easy for users to use the model for practical, real-time wildfire detection tasks.
