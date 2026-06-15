# Loan Approval Prediction Using Artificial Neural Networks (ANN) with TensorFlow

## Assignment Overview

This Assignment uses an **Artificial Neural Network (ANN)** built with **TensorFlow/Keras** to predict whether a loan application will be **Approved** or **Rejected** based on applicant information.

The complete deep learning workflow includes data exploration, preprocessing, feature selection, model training, evaluation, and prediction.

---

# Assignment Workflow

## Importing Libraries

The following libraries are used in this assignment:

- Pandas
- NumPy
- Warnings
- Scikit-learn (sklearn)
- TensorFlow

---

## Data Exploration

- Loading the dataset
- Checking duplicate records
- Checking missing values
- Checking data types
- Understanding dataset structure

---

## Data Preprocessing

- Dropping unnecessary columns
- Converting categorical values into numerical values
- Preparing data for machine learning

---

## Feature Selection

- Correlation analysis
- Selecting important features for prediction

---

## Splitting Features and Target

### Features (X)
Input variables used for prediction.

### Target (y)
Loan approval status.

---

## Feature Scaling

A **StandardScaler** is applied to the feature set.

### Benefits

- Standardizes feature values
- Improves model performance
- Helps the ANN learn patterns more efficiently
- Speeds up convergence during training

---

## Train-Test Split

- **80% Training Data**
- **20% Testing Data**

---

## ANN Model Architecture

### Hidden Layer 1
- 64 Neurons
- ReLU Activation Function

### Hidden Layer 2
- 16 Neurons
- ReLU Activation Function

### Hidden Layer 3
- 8 Neurons
- ReLU Activation Function

### Output Layer
- 2 Neurons
- Softmax Activation Function
- Used for Binary Classification

---

## Model Compilation

- Optimizer: RMSprop
- Loss Function: SparseCategoricalCrossentropy
- Evaluation Metric: Accuracy

---

## Model Training

The model is trained using scaled training features and corresponding target labels.

---

## Model Evaluation

### Results

- Testing Accuracy: **95%**
- Strong Generalization Performance
- Reliable Predictions on Unseen Data

---

## Model Summary

| Property | Value |
|-----------|---------|
| Total Parameters | 3,926 |
| Hidden Layers | 3 |
| Hidden Layer Neurons | 64 → 16 → 8 |
| Output Neurons | 2 |
| Activation Functions | ReLU, Softmax |

---

## Loan Approval Prediction Function

```
predict_loan_approval()
```

### Function Workflow

1. Accepts user input
2. Applies preprocessing and scaling
3. Passes data to the trained ANN model
4. Predicts loan approval status
5. Returns:
   - Predicted Class
   - Prediction Confidence Score

---

# Model Performance

| Metric | Score |
|----------|----------|
| Testing Accuracy | 95% |
| Classification Type | Binary Classification |
| Framework | TensorFlow/Keras |
| Model Type | Artificial Neural Network (ANN) |

---

# Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow
- Keras

---
