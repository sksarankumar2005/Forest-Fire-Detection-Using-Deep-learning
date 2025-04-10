# Forest-Fire-Detection-Using-Deep-learning
# WEEK 2
1. Data Acquisition and Setup 🔍🧠

I started off by using kagglehub to download the Wildfire Dataset from Kaggle.
Then, I imported all the necessary libraries like os, numpy, matplotlib, tensorflow, etc. 🧰
I also checked if a GPU was available to speed up training ⚡
Next, I defined the paths to my training, validation, and testing datasets so everything was well organized 📁

2. Data Exploration 🔥🖼️

I listed out the classes (fire and no_fire) and checked how many images each class had.
To get a feel for the data, I visualized a few sample images from both categories.
Also, I printed the shape of the images to understand their dimensions 📐

3. Data Preprocessing 🧹📊

I set the image height and width, and chose a good batch size.
Then, I created ImageDataGenerator instances to rescale pixel values to the [0, 1] range.
Using flow_from_directory, I generated image batches for training, validation, and testing.
Finally, I mapped class indices to their actual names for easier interpretation 🧠

4. Model Building 🏗️🤖

I built a Convolutional Neural Network (CNN) using keras.Sequential. Here's what the model includes:

An input layer to take in the images

Multiple Conv2D layers to extract important features 🧬

MaxPooling2D layers to reduce spatial dimensions

A Flatten layer to convert everything into a single vector

Dense layers for learning and classification

A Dropout layer to help prevent overfitting 💧

And finally, an output layer with a sigmoid activation for binary classification (fire 🔥 or no fire 🌲)
