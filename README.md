# House Price Prediction Using Linear Regression

This repository contains a **machine learning–based house price prediction system** built using **Linear Regression from scikit-learn**.  
The project focuses on real-world data preprocessing, feature scaling, log transformation, model evaluation, and prediction on new unseen inputs.

Unlike a scratch implementation, this project emphasizes **practical ML workflow and industry-standard tools**.

---

## 📌 Project Overview

The objective of this project is to predict **house prices** using property-related features extracted from a real dataset.  
The model is trained using Linear Regression and evaluated using standard regression metrics.

---

## 🏠 Dataset

- Dataset: `Islamabad_zameen.csv`
- Separator: `|`
- Source: Real estate listing data (Islamabad region)

### Features Used
- `size` — Property size
- `bedrooms` — Number of bedrooms
- `baths` — Number of bathrooms

### Target Variable
- `price` — House price

---

## 🔍 Data Preprocessing

The following preprocessing steps are applied:

- Missing value inspection using heatmaps
- Feature standardization (mean normalization & standard deviation)
- Log transformation of the target variable to reduce skewness
- Feature-target separation
- Train-test split (70% training, 30% testing)

---

## 📊 Exploratory Data Analysis

- Heatmap visualization for missing values
- Scatter plots to analyze relationships between features and house prices
- Comparison of raw vs normalized feature distributions

---

## ⚙️ Model Implementation

- Algorithm: **Linear Regression**
- Library: `scikit-learn`
- Train-test split ratio: **70 / 30**

The model is trained on standardized features and evaluated on unseen test data.

---

## 📈 Model Evaluation Metrics

The following metrics are used to assess model performance:

- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**
- **R² Score (Coefficient of Determination)**

These metrics provide insight into prediction accuracy and error magnitude.

---

## 🧪 Prediction on New Data

The project also supports **predicting prices for new houses** by:

1. Applying the same feature scaling used during training
2. Generating predictions using the trained model
3. Converting predictions back from log scale to original price values
```python
new_house = [[420, 0, 0]]
