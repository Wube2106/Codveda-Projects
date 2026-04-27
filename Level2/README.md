# 📊 Machine Learning Projects Collection

This repository contains three machine learning tasks implemented using **Python**, **pandas**, and **scikit-learn**. The projects demonstrate both **supervised and unsupervised learning**, including classification, regression-style interpretation, and clustering.

---

#  Project Structure

```
├── Task 1: Logistic Regression (Churn Prediction)
├── Task 2: Decision Tree Classification (Iris Dataset)
├── Task 3: K-Means Clustering (Iris Dataset)
├── datasets/
└── README.md
```

---

#  Task 1: Logistic Regression (Churn Prediction)

##  Objective
Build a binary classification model to predict whether a customer will churn or not.

##  Steps Performed
- Loaded churn dataset
- Handled missing values and duplicates
- Encoded categorical features
- Applied feature scaling
- Split data into training and testing sets
- Trained **Logistic Regression model**
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - Confusion Matrix
  - ROC Curve and AUC

##  Results
- Accuracy: ~72%
- Good recall for detecting churn customers
- AUC ≈ 0.78 shows strong classification ability

##  Insight
- Customer service calls strongly increase churn probability
- Voice mail plan reduces churn likelihood

##  Tools Used
- pandas
- scikit-learn (LogisticRegression, metrics)
- matplotlib

#  Task 2: Decision Tree Classification (Iris Dataset)

##  Objective
Classify Iris flower species using a Decision Tree model.

##  Steps Performed
- Loaded Iris dataset
- Removed duplicates
- Split features and target variable
- Train-test split
- Trained **Decision Tree Classifier**
- Applied **pre-pruning (max_depth = 3)**
- Visualized decision tree
- Evaluated using:
  - Accuracy
  - F1-score
  - Confusion Matrix

##  Results
- Accuracy: ~90%
- Good performance across all classes
- Minor confusion between Versicolor and Virginica

##  Insight
- Pre-pruning helped reduce overfitting
- Model is highly interpretable through tree visualization

##  Tools Used
- pandas
- scikit-learn (DecisionTreeClassifier)
- matplotlib


#  Task 3: K-Means Clustering (Iris Dataset)

##  Objective
Group Iris flowers into clusters using unsupervised learning.

##  Steps Performed
- Loaded Iris dataset
- Removed duplicates
- Dropped target column (`species`)
- Applied feature scaling
- Used **Elbow Method** to find optimal K
- Trained **K-Means clustering model**
- Reduced dimensions using PCA
- Visualized clusters and centroids

##  Results
- Optimal K selected using elbow method
- Clear cluster separation in 2D PCA plot
- Centroids correctly represent cluster centers

##  Insight
- K-Means successfully groups similar flowers without labels
- PCA helps in visualizing high-dimensional data

##  Tools Used
- pandas
- scikit-learn (KMeans, PCA)
- seaborn, matplotlib

#  Conclusion

This project demonstrates a full machine learning workflow:

- Data preprocessing
- Supervised learning (Logistic Regression & Decision Tree)
- Unsupervised learning (K-Means Clustering)
- Model evaluation and visualization

It builds a strong foundation in practical machine learning concepts.