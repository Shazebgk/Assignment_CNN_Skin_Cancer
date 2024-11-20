# Assignment_CNN_Skin_Cancer

CNN Skin Cancer Detection
A machine learning project to develop a custom convolutional neural network (CNN) model for accurately detecting melanoma, a type of skin cancer, using a dataset of skin lesion images.

Table of Contents
General Info
Technologies Used
Conclusions
Acknowledgements
General Information
Skin cancer, especially melanoma, is a critical health issue, responsible for 75% of skin cancer-related deaths. Early detection is crucial in reducing mortality rates. This project aims to create a multiclass classification CNN model capable of identifying skin lesions from dermoscopic images and detecting melanoma among other types of oncological diseases.

Business Problem
The objective is to build a model that can:

Assist dermatologists in diagnosing melanoma early and accurately.
Reduce manual effort by automating the classification of skin lesions into nine categories.

Dataset
The dataset consists of 2,357 images of malignant and benign skin lesions derived from the International Skin Imaging Collaboration (ISIC). The images are categorized into the following nine classes:

Actinic Keratosis
Basal Cell Carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented Benign Keratosis
Seborrheic Keratosis
Squamous Cell Carcinoma
Vascular Lesion
Project Pipeline

Data Reading/Understanding:
Define paths for the training and testing datasets.

Dataset Creation:
Split the dataset into training and validation sets with a batch size of 32.
Resize images to 180x180 pixels.

Dataset Visualization:
Visualize one image instance from each of the nine classes.

Model Building and Initial Training:
Build a custom CNN model to classify the nine categories.
Normalize pixel values between 0 and 1.
Train the model for 20 epochs using an appropriate optimizer and loss function.
Analyze the results for signs of overfitting or underfitting.

Data Augmentation:
Apply augmentation techniques to resolve overfitting or underfitting issues.
Model Training on Augmented Data:
Retrain the model with augmented data for improved performance.
Evaluate if the earlier issues were resolved.

Class Distribution Analysis:
Examine the distribution of classes to identify imbalance.

Handling Class Imbalances:
Use the Augmentor library to rectify imbalances.

Final Model Training:
Retrain the model after balancing the dataset.
Train the model for 30 epochs and evaluate results.


Findings:
Provide insights on the final performance and resolutions to identified issues.
Conclusions
The model successfully classifies images into nine categories with improved accuracy after augmentation and handling class imbalance.
Class imbalances were addressed effectively, enhancing model performance for underrepresented classes.
Data augmentation significantly reduced overfitting and improved generalization.
The final model demonstrates robustness in detecting melanoma and other skin conditions.
Technologies Used
Python: Programming language for model development.
TensorFlow/Keras: Framework for building and training CNN models.
Augmentor: Library for handling data augmentation and class imbalance.
Google Colab: Environment for training the model with GPU support.
Matplotlib: Visualization of dataset samples and performance metrics.
Acknowledgements
This project was inspired by real-world challenges in dermatology and cancer diagnosis.
Dataset courtesy of the International Skin Imaging Collaboration (ISIC).
The project builds on foundational concepts of deep learning and CNNs.


Contact
Created by @Shazebgk – Feel free to reach out for collaboration or inquiries!
