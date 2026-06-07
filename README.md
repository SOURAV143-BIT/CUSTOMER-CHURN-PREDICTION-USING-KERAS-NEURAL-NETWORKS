# Customer Churn Prediction Using Keras Neural Networks

## Project Overview

Customer churn is one of the biggest challenges faced by telecom companies. Customer churn occurs when customers stop using a company's services and move to competitors. Predicting customer churn helps businesses identify at-risk customers and take preventive actions to improve customer retention.

In this project, machine learning and deep learning techniques are used to analyze telecom customer data and predict whether a customer is likely to churn.

---

## Dataset

The dataset contains customer information from a telecom company, including demographic details, account information, service subscriptions, and billing data.

### Key Features

* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Phone Service
* Internet Service
* Contract Type
* Payment Method
* Monthly Charges
* Total Charges
* Churn (Target Variable)

---

## Objectives

* Perform data manipulation and customer analysis.
* Visualize customer churn trends.
* Build Artificial Neural Network (ANN) models using Keras.
* Compare different neural network architectures.
* Evaluate model performance using confusion matrices and accuracy metrics.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* TensorFlow
* Keras
* Jupyter Notebook

---

## Project Tasks

### Data Manipulation

* Calculated total number of male customers.
* Identified customers using DSL internet service.
* Extracted female senior citizens using mailed check payment method.
* Extracted customers with:

  * Tenure less than 10 months
  * Total charges less than $500

### Data Visualization

* Pie Chart showing customer churn distribution.
* Bar Plot showing internet service distribution.

---

## Model 1: ANN Using Tenure

### Architecture

Input Layer:

* 12 Neurons
* ReLU Activation

Hidden Layer:

* 8 Neurons
* ReLU Activation

Output Layer:

* 1 Neuron
* Sigmoid Activation

### Training Configuration

* Optimizer: Adam
* Loss Function: Binary Crossentropy
* Epochs: 150

### Evaluation

* Confusion Matrix
* Accuracy Score
* Accuracy vs Epochs Graph

---

## Model 2: ANN with Dropout Layers

### Additional Regularization

* Dropout Layer (0.3) after Input Layer
* Dropout Layer (0.2) after Hidden Layer

### Purpose

Dropout is used to reduce overfitting and improve model generalization.

### Evaluation

* Confusion Matrix
* Accuracy Score
* Accuracy vs Epochs Graph

---

## Model 3: ANN Using Multiple Features

### Features Used

* Tenure
* Monthly Charges
* Total Charges

### Architecture

Input Layer:

* 12 Neurons
* ReLU Activation

Hidden Layer:

* 8 Neurons
* ReLU Activation

Output Layer:

* 1 Neuron
* Sigmoid Activation

### Training Configuration

* Optimizer: Adam
* Epochs: 150

### Evaluation

* Confusion Matrix
* Accuracy Score
* Accuracy vs Epochs Graph

---

## Results

The third model achieved the best performance because it utilized multiple customer-related features instead of relying solely on tenure.

### Performance Comparison

| Model   | Features Used                            | Expected Accuracy |
| ------- | ---------------------------------------- | ----------------- |
| Model 1 | Tenure                                   | 73% - 77%         |
| Model 2 | Tenure + Dropout                         | 73% - 77%         |
| Model 3 | Tenure + Monthly Charges + Total Charges | 78% - 83%         |

---

## Key Learnings

* Data preprocessing and feature engineering.
* Customer churn analysis.
* Building Artificial Neural Networks using Keras.
* Using Dropout layers to prevent overfitting.
* Model evaluation using confusion matrices.
* Visualizing model performance through learning curves.

---

## Conclusion

This project demonstrates how Deep Learning can be applied to solve real-world customer retention problems in the telecom industry. By predicting customer churn, businesses can identify customers at risk of leaving and implement targeted retention strategies.

The project also provides hands-on experience with TensorFlow, Keras, data preprocessing, visualization, and neural network model development.
