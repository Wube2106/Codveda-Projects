# 📊 Machine Learning & Deep Learning Projects Collection

This repository contains three machine learning and deep learning tasks implemented using **Python**, **pandas**, **scikit-learn**, and **TensorFlow/Keras**. The projects demonstrate **supervised learning and deep learning**, including classification, model tuning, and neural networks.

---

#  Project Structure

```
├── Task 1: Random Forest Classification (Iris Dataset)
├── Task 2: Support Vector Machine (Churn Prediction)
├── Task 3: Neural Network (MNIST Dataset)
├── datasets/
└── README.md
```i


# Task 1: Random Forest Classification (Iris Dataset)

## Objective
Build a multi-class classification model to predict Iris flower species using Random Forest.

## 🧩 Steps Performed
- Loaded Iris dataset
- Handled missing values and duplicates
- Split features and target variable
- Train-test split
- Trained **Random Forest Classifier**
- Performed **hyperparameter tuning (GridSearchCV)**
- Evaluated using:
  - Accuracy     - F1-score          - Precision
  - Recall       - Confusion Matrix  - Cross-validation
  
- Feature importance analysis

##  Results
- High accuracy after tuning (~95%+)
- Strong and stable performance
- Very few misclassifications

##  Tools Used
- pandas
- scikit-learn (RandomForestClassifier, GridSearchCV)
- matplotlib

---

# Task 2: Support Vector Machine (Churn Prediction)

## 🎯 Objective
Predict customer churn using SVM models and compare Linear vs RBF kernel.

## 🧩 Steps Performed
- Loaded churn dataset
- Handled missing values and duplicates
- Encoded categorical variables
- Feature scaling using StandardScaler
- Train-test split
- Trained:
  - Linear SVM
  - RBF SVM
- Evaluated using:
  - Accuracy   - Precision
  - Recall     - AUC Score
- PCA used for visualization

##  Results
- RBF SVM achieved higher accuracy
- Linear SVM performed better in recall
- Strong AUC score

##  Tools Used
- pandas, numpy
- scikit-learn (SVC, PCA, metrics)
- matplotlib

---

#  Task 3: Neural Network (MNIST Dataset)

##  Objective
Classify handwritten digits (0–9) using a feed-forward neural network.

##  Steps Performed
- Loaded MNIST dataset
- Normalized pixel values (0–255 → 0–1)
- Built neural network using Keras:
  - Flatten layer
  - Dense hidden layers (ReLU)
  - Output layer (Softmax)
- Compiled model using Adam optimizer
- Trained using backpropagation
- Evaluated using:
  - Accuracy
  - Loss curves
  - Confusion Matrix
- Made predictions on test data

##  Results
- High accuracy (~97–98%)
- Stable training performance
- Strong classification results

## Tools Used
- TensorFlow / Keras    - numpy
- scikit-learn         - matplotlib  

---

# Conclusion

This project demonstrates a complete machine learning workflow:

- Data preprocessing
- Supervised learning (Random Forest, SVM)
- Deep learning (Neural Networks)
- Model evaluation and visualization

It provides strong hands-on experience in both classical ML and deep learning.
