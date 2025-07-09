# SONAR Data Classification: Rock or Mine Prediction

## Project Overview

This project implements a predictive model using Logistic Regression to classify objects as either Rock or Mine based on SONAR data. The dataset consists of various features that represent SONAR readings, and the model aims to accurately predict the type of object based on these readings.

## Table of Contents

- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Steps Involved](#steps-involved)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Making Predictions](#making-predictions)

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook

## Dataset

The dataset used in this project is the **sonar data.csv** file, which contains **208 samples** with **60 features** each. The last column indicates the class label:
- **M**: Mine
- **R**: Rock

## Steps Involved

1. **Importing Dependencies**: Load necessary libraries for data manipulation and model training.
   
2. **Data Collection and Processing**:
   - Load the dataset into a Pandas DataFrame.
   - Analyze the dataset to understand its structure and check for missing values.

3. **Data Separation**: Separate the features (X) and labels (Y) for model training.

4. **Train-Test Split**: Split the dataset into training and testing sets using a stratified approach.

5. **Model Training**: Train a Logistic Regression model using the training data.

6. **Model Evaluation**: Evaluate the model's accuracy on both training and test datasets.

7. **Making Predictions**: Create a predictive system to classify new SONAR readings.

## Model Training

The Logistic Regression model is trained using the training dataset. The model is fitted to the data, allowing it to learn the relationship between the features and the labels.

## Model Evaluation

- **Training Data Accuracy**: The model achieved an accuracy of **83.42%** on the training data.
- **Test Data Accuracy**: The model achieved an accuracy of **76.19%** on the test data.

## Making Predictions

The model can predict whether an object is a Rock or Mine based on new SONAR readings. For example, given the input data:

```python
input_data = (0.0307, 0.0523, 0.0653, 0.0521, 0.0611, 0.0577, 0.0665, 0.0664, 0.1460, 0.2792, 0.3877, 0.4992, 0.4981, 0.4972, 0.5607, 0.7339, 0.8230, 0.9173, 0.9975, 0.9911, 0.8240, 0.6498, 0.5980, 0.4862, 0.3150, 0.1543, 0.0989, 0.0284, 0.1008, 0.2636, 0.2694, 0.2930, 0.2925, 0.3998, 0.3660, 0.3172, 0.4609, 0.4374, 0.1820, 0.3376, 0.6202, 0.4448, 0.1863, 0.1420, 0.0589, 0.0576, 0.0672, 0.0269, 0.0245, 0.0190, 0.0063, 0.0321, 0.0189, 0.0137, 0.0277, 0.0152, 0.0052, 0.0121, 0.0124, 0.0055)
