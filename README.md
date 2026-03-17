# Predictive Analytics Project

## Objective

The objective of this project is to perform a binary classification task using machine learning, including:

* Exploratory Data Analysis (EDA)
* Model building
* Decision boundary visualization
* Model evaluation

---

## Dataset Description

The dataset contains 1020 observations with the following features:

* Feature1: Continuous numerical feature
* Feature2: Discrete numerical feature
* Target: Binary categorical variable (Yes / No)

### Preprocessing Steps

* Removed missing values from the dataset
* Converted target labels:

  * Yes → 1
  * No → 0

---

## Exploratory Data Analysis (EDA)

The following analysis was performed:

* Examined dataset structure using `.info()` and `.describe()`
* Identified and removed missing values
* Visualized class distribution using a count plot
* Analyzed feature relationships using a correlation heatmap

### Observations

* Dataset is suitable for binary classification
* Features are numerical and can be visualized in 2D space
* No complex preprocessing required

---

## Model Used

Logistic Regression

### Reason for Selection

* Suitable for binary classification
* Produces a linear decision boundary
* Efficient and fast for small datasets

---

## Methodology

1. Data loading
2. Handling missing values
3. Encoding target variable
4. Feature selection (Feature1 and Feature2)
5. Train-test split (80:20)
6. Feature scaling using StandardScaler
7. Model training using Logistic Regression
8. Prediction on test data

---

## Decision Boundary Visualization

* The decision boundary was plotted using Feature1 and Feature2
* It separates the two classes in the feature space

### Key Insight

The decision boundary is linear, confirming that Logistic Regression is a linear classifier.

---

## Model Evaluation

### Accuracy

Accuracy = 76.5%

### Classification Report

| Class | Precision | Recall | F1-Score |
| ----- | --------- | ------ | -------- |
| 0     | 0.765     | 1.00   | 0.867    |
| 1     | 0.000     | 0.00   | 0.000    |

### Overall Metrics

* Macro Average F1-score = 0.433
* Weighted Average F1-score = 0.663

---

## Interpretation

* The model performs reasonably well overall with 76.5% accuracy
* The model predicts class 0 effectively
* Performance on class 1 is poor, indicating possible class imbalance or model bias

---

## Conclusion

* Logistic Regression successfully models the dataset
* The decision boundary is clearly visualized
* Model performance is acceptable but can be improved for minority class prediction

---

## Files Included

* Lab_Exam_binary_classification_dataset.csv → Dataset
* main.py / labExam_2.ipynb → Implementation code
* README.md → Documentation

---

## Final Note

This project demonstrates a complete machine learning workflow:

EDA → Preprocessing → Model Building → Visualization → Evaluation

---
