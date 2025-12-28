# 💳 Credit Card Customer Churn Prediction

## 📌 Project Overview

Customer churn prediction is a critical task for banks to retain high-value customers and reduce revenue loss.  
This project focuses on analyzing customer behavior using **Exploratory Data Analysis (EDA)** and building an **Artificial Neural Network (ANN)** to predict whether a credit card customer is likely to **exit (churn)** or not.

The project follows a structured **Machine Learning workflow**:

- Data Understanding  
- Exploratory Data Analysis  
- Data Preprocessing  
- Neural Network Model Building  
- Model Training & Evaluation  

---

## 🎯 Objective

To predict customer churn using demographic and behavioral attributes and understand **why customers leave the bank**.

### 🎯 Target Variable

- **Exited**
  - `1` → Customer churned  
  - `0` → Customer retained  

---

## 📊 Dataset Description

The dataset contains customer information related to banking behavior.

### 📋 Key Features

| Feature | Description |
|--------|------------|
| CreditScore | Credit score of the customer |
| Geography | Customer’s country |
| Gender | Male / Female |
| Age | Age of the customer |
| Balance | Account balance |
| NumOfProducts | Number of bank products used |
| HasCrCard | Whether customer has a credit card |
| IsActiveMember | Customer activity status |
| EstimatedSalary | Estimated annual salary |
| Exited | Churn indicator (Target) |

---

## 🔍 Exploratory Data Analysis (EDA)

### ✅ Univariate Analysis
- Performed univariate analysis on the input data to see the distribution (histogram and boxplot for numerical cols), bar plot and pie chart for categorical columns. The target variable **Exited** shows
imbalanced distribution.
---

### ✅ Bivariate Analysis
- Performed bivariate analysis of **Exited** column with other input columns.

---

### ✅ Multivariate Analysis
- A correlation analysis was performed to identify relationships between multiple features and **Exited**.
- Most other features exhibit weak linear correlation, suggesting churn is influenced by **complex feature interactions**

---

## ⚙️ Data Preprocessing

Steps applied before modeling:

- One-Hot Encoding for categorical variables (`Geography`, `Gender`)
- Feature scaling using **StandardScaler**
- Train–Test split for unbiased model evaluation

---

## 🤖 Artificial Neural Network (ANN)

### 🔹 Model Architecture
- Input Layer (scaled features)
- Hidden Layers with **ReLU activation**
- Output Layer with **Sigmoid activation** (binary classification)

---

### 🔹 Framework Used
- **TensorFlow (Keras API)**

---

### 🔹 Loss & Optimizer
- **Loss Function:** Binary Crossentropy  
- **Optimizer:** Adam  
- **Metric:** Accuracy  

---

## 📈 Model Training & Evaluation

- Model trained over multiple epochs
- Validation split used to monitor overfitting
- Performance evaluated on unseen test data

The ANN effectively captures **non-linear relationships and feature interactions**, outperforming traditional linear models for this problem.
