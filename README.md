# Logistic Regression – Breast Cancer Detection

This project demonstrates the use of **Logistic Regression** to classify breast cancer tumors as **benign** or **malignant** using a real dataset. The workflow includes data preprocessing, feature scaling, model training, evaluation, and visualization.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Libraries Used](#libraries-used)
4. [Data Preprocessing](#data-preprocessing)
5. [Model Training](#model-training)
6. [Predictions and Evaluation](#predictions-and-evaluation)
7. [k-Fold Cross Validation](#k-fold-cross-validation)
8. [Decision Boundary Visualization](#decision-boundary-visualization)
9. [Usage](#usage)
10. [Results](#results)

---

## Project Overview
We build a **Logistic Regression** model to classify tumors as **benign (0)** or **malignant (1)**. The dataset contains 9 features describing cell characteristics. 

---

## Dataset
The dataset used is `breast_cancer.csv` which includes the following features:

- Clump Thickness  
- Uniformity of Cell Size  
- Uniformity of Cell Shape  
- Marginal Adhesion  
- Single Epithelial Cell Size  
- Bare Nuclei  
- Bland Chromatin  
- Normal Nucleoli  
- Mitoses  
- Class (target variable)

The **ID column** (`Sample code number`) is dropped during preprocessing.

---

## Libraries Used
- numpy  
- pandas  
- matplotlib  
- sklearn: `LogisticRegression`, `StandardScaler`, `train_test_split`, `cross_val_score`, `confusion_matrix`, `classification_report`

---

## Data Preprocessing
- Convert class labels from (2, 4) to (0, 1)  
- Split dataset into **training (80%)** and **testing (20%)** sets  
- Apply **feature scaling** using `StandardScaler`

---

## Model Training
We train a **Logistic Regression** classifier using the training set and predict the test set labels.

---

## Predictions and Evaluation
We evaluate the model using:

- **Confusion Matrix**  
- **Accuracy Score**  
- **Classification Report** (Precision, Recall, F1-Score)

We also display a table comparing **predicted vs actual labels**.

---

## k-Fold Cross Validation
We evaluate the model stability using **10-fold cross-validation** on the training set.  
This helps assess the variance and robustness of the model.

---

## Decision Boundary Visualization
We plot the decision boundary for **training** and **test** sets using the first two features:  
- **Clump Thickness** (X-axis)  
- **Uniformity of Cell Size** (Y-axis)

This visualization shows how the classifier separates benign and malignant tumors.

---
