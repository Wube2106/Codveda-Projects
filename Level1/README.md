# 📊 Machine Learning Projects Collection

This repository contains three machine learning tasks implemented using **Python**, **pandas**, and **scikit-learn**. The projects demonstrate core concepts including **data preprocessing**, **classification (KNN)**, and **regression (Linear Regression)**.

---

#  Project Structure

```
├── Task 1: Data Preprocessing
├── Task 2: Linear Regression Model
├── Task 3: KNN Classifier (Iris Dataset)
├── datasets/
└── README.md
```

---

#  Task 1: Data Preprocessing for Machine Learning

##  Objective

Prepare raw data for machine learning by handling missing values, encoding categorical variables, scaling features, and splitting the dataset.

##  Steps Performed

* Loaded stock price dataset
* Handled missing values:

  * Mean for price columns
  * Median for volume
* Removed duplicate records
* Encoded categorical variable (`symbol`) using Label Encoding
* Converted `date` column to datetime
* Applied **Standard Scaling**
* Split dataset into training and testing sets (without shuffling for time-series)

##  Tools Used

* pandas
* scikit-learn (StandardScaler, LabelEncoder)

---

#  Task 2: Simple Regression Model

##  Objective

Build a regression model to predict stock closing prices.

##  Steps Performed

* Data cleaning (missing values & duplicates)
* Feature selection (excluded `symbol` and `date`)
* Train-test split (time-series aware, no shuffle)
* Trained **Linear Regression model**
* Evaluated using:

  * Mean Squared Error (MSE)
  * R² Score
* Visualized actual vs predicted values

##  Results

* Very low MSE → accurate predictions
* R² close to 1 → strong model fit
* Model captures trend effectively

##  Note

High R² may indicate potential overfitting, so careful validation is recommended for future work.

##  Tools Used

* pandas
* scikit-learn (LinearRegression)
* matplotlib & seaborn

---

#  Task 3: KNN Classifier (Iris Dataset)

##  Objective

Train a classification model using K-Nearest Neighbors (KNN) and compare performance for different values of K.

##  Steps Performed

* Loaded Iris dataset
* Checked and removed duplicates
* Split features and target (`species`)
* Applied **Standard Scaling**
* Trained KNN model with different K values:

  * K = 1, 3, 5, 7, 15
* Evaluated using:

  * Accuracy
  * Precision (macro)
  * Recall (macro)
  * Confusion Matrix

##  Results

* Accuracy ≈ **93.3%** across multiple K values
* Very small number of misclassifications
* Similar performance for K = 3, 5, 7 due to dataset simplicity

##  Insight

The Iris dataset is well-separated, so changing K does not significantly affect performance. Predictions remain consistent across multiple values of K.

## 🛠 Tools Used

* python
* pandas
* scikit-learn (KNeighborsClassifier, metrics)

---

#  Conclusion

This project demonstrates a complete machine learning workflow:

* Data preprocessing
* Model building
* Evaluation
* Comparison

It provides a strong foundation for understanding practical ML concepts.

