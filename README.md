# AI & ML Task 4 – Classification Models, Evaluation Metrics & Handling Imbalanced Data

## Project Overview

This project was completed as part of an Artificial Intelligence & Machine Learning internship program.

The objective of this project is to build and evaluate binary classification models using the Breast Cancer Wisconsin Dataset from Scikit-learn. The project focuses on model evaluation, ROC-AUC analysis, class imbalance handling, and model comparison.

---

## Dataset

**Breast Cancer Wisconsin Dataset**

Source: Scikit-learn Built-in Dataset

Target Classes:

- 0 → Malignant
- 1 → Benign

Dataset Size:

- 569 Samples
- 30 Features

---

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Project Workflow

### 1. Data Loading

The Breast Cancer dataset was loaded using Scikit-learn.

### 2. Data Splitting

The dataset was divided into training and testing sets using stratified sampling to preserve class distribution.

### 3. Feature Scaling

StandardScaler was applied to normalize the features before training Logistic Regression.

### 4. Logistic Regression Model

A Logistic Regression classifier was trained and used as the baseline model.

### 5. Model Evaluation

The model was evaluated using:

- Confusion Matrix
- Accuracy
- Precision
- Recall
- F1-Score
- ROC Curve
- AUC Score

### 6. ROC Curve Analysis

ROC Curve and AUC Score were used to measure the model's ability to distinguish between classes.

### 7. Handling Class Imbalance

Class imbalance was addressed using:

```python
class_weight='balanced'
```

### 8. Model Comparison

A Decision Tree Classifier was trained and compared with Logistic Regression.

---

## Logistic Regression Results

### Confusion Matrix

```text
[[41  1]
 [ 1 71]]
```

### Classification Report

| Metric | Class 0 | Class 1 |
|----------|----------|----------|
| Precision | 0.98 | 0.99 |
| Recall | 0.98 | 0.99 |
| F1-Score | 0.98 | 0.99 |

### Overall Accuracy

```text
98%
```

### ROC-AUC Score

```text
0.995
```

---

## Decision Tree Results

| Metric | Class 0 | Class 1 |
|----------|----------|----------|
| Precision | 0.85 | 0.96 |
| Recall | 0.93 | 0.90 |
| F1-Score | 0.89 | 0.93 |

### Overall Accuracy

```text
91%
```

---

## Model Comparison

| Feature | Logistic Regression | Decision Tree |
|----------|----------|----------|
| Accuracy | 98% | 91% |
| Precision | Higher | Lower |
| Recall | Higher | Lower |
| F1-Score | Higher | Lower |
| Overfitting Risk | Low | Higher |
| Generalization | Better | Moderate |

---

## Why Accuracy Alone Is Not Enough

Accuracy may be misleading when classes are imbalanced. Therefore, Precision, Recall, and F1-Score were also used to evaluate model performance.

---

## Importance of Recall in Medical Diagnosis

Recall is especially important in medical diagnosis because failing to detect a positive case can lead to serious consequences.

A low recall value means some disease cases may not be identified correctly.

---

## Why F1-Score Is Important

F1-Score provides a balance between Precision and Recall and is particularly useful for imbalanced datasets.

---

## Handling Imbalanced Data

Class imbalance is a common challenge in real-world classification problems.

Using:

```python
class_weight='balanced'
```

helps the model pay additional attention to minority-class samples and improves fairness in prediction.

---

## Final Model Decision

Logistic Regression achieved:

- 98% Accuracy
- Excellent Precision
- Excellent Recall
- Excellent F1-Score
- AUC Score of 0.995

Decision Tree achieved:

- 91% Accuracy

Based on the evaluation results, Logistic Regression was selected as the final model because it demonstrated superior performance, better generalization, and lower risk of overfitting.

---

## Repository Contents

```text
AI_ML_Task4_Classification_Evaluation.ipynb
README.md
AI_ML_Task4_All_Deliverables.pdf
```

---

## Author

Haider Altahir

Mechanical Engineering Student  
Andhra University, India
