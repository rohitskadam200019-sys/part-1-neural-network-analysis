# Part 1: Neural Network Fundamentals and Training Behavior Analysis

## Project Overview

This project focuses on building and analyzing a feed-forward neural network model for customer churn prediction using a structured dataset. The objective of the project is to understand how neural networks learn through forward propagation, loss calculation, backpropagation, and parameter optimization.

The model predicts whether a customer is likely to churn or remain retained based on multiple customer-related features.

---

# Dataset Information

Dataset Used: `customer_churn_nn.csv`

## Target Variable
- `churn`
  - `1` = Customer Churned
  - `0` = Customer Retained

## Feature Types

### Categorical Features
- region
- plan_type
- contract_type
- payment_method

### Numerical Features
- tenure
- charges
- login days
- tickets
- delays
- data usage
- satisfaction
- complaint recency
- discounts
- referrals

### Removed Column
- customer_id (identifier column)

---

# Tasks Performed

## Task 1: Dataset Understanding
- Loaded and explored the dataset
- Checked dataset shape and feature types
- Performed missing value analysis
- Generated statistical summary
- Visualized target variable distribution

---

## Task 2: Data Preprocessing
- Removed unnecessary identifier column
- Encoded categorical variables using LabelEncoder
- Scaled numerical features using StandardScaler
- Split dataset into training and testing sets

---

## Task 3: Neural Network Model Building
A feed-forward neural network was created using TensorFlow/Keras.

### Model Architecture
- Input Layer
- Hidden Layer 1 → 64 neurons with ReLU activation
- Hidden Layer 2 → 32 neurons with ReLU activation
- Output Layer → 1 neuron with Sigmoid activation

### Loss Function
- Binary Crossentropy

### Optimizer
- Adam Optimizer

---

## Task 4: Training and Evaluation
The model was trained and evaluated using:
- Training Accuracy
- Training Loss
- Testing Accuracy
- Testing Loss
- Confusion Matrix

The confusion matrix was used to evaluate prediction performance on churn classification.

---

## Task 5: Hyperparameter Experimentation
Three different experiments were performed by modifying:
- Number of hidden layers
- Number of neurons
- Activation functions
- Epochs
- Batch size

A comparison table was created to analyze the effect of different hyperparameters on model performance.

---

## Task 6: Final Reflection
The project also includes theoretical explanations covering:
- Role of weights and biases
- Importance of activation functions
- Effect of learning rate
- Underfitting and overfitting

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras

---
# Conclusion

The project successfully demonstrated the implementation of a feed-forward neural network for customer churn prediction. The neural network was able to learn meaningful patterns from the dataset and provide reasonable classification performance. Hyperparameter experimentation further helped in understanding the effect of model configuration on performance.
