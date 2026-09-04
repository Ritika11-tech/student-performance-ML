# 📊 Student Performance Prediction & Model Evaluation

## 📌 Project Overview

This project focuses on analyzing student performance data and building Machine Learning models to understand and predict students' exam performance.

The project follows a complete Machine Learning workflow, starting with **Exploratory Data Analysis (EDA)**, followed by **data preprocessing, regression, classification, model evaluation, and analysis of overfitting/underfitting**.

The main objective is to identify the factors that influence students' exam scores and use Machine Learning techniques to predict student performance.

---

## 🎯 Objectives

* Perform Exploratory Data Analysis (EDA) on the Student Performance dataset.
* Identify numerical and categorical variables.
* Analyze distributions, relationships, correlations, missing values, and outliers.
* Identify factors related to students' exam scores.
* Build a **Linear Regression model** to predict `exam_score`.
* Convert exam scores into **Pass/Fail categories** using 50 marks as the passing threshold.
* Build a **Logistic Regression classification model**.
* Evaluate regression and classification models using appropriate metrics.
* Compare training and testing performance.
* Identify possible signs of overfitting or underfitting.
* Derive meaningful insights about student performance.

---

## 📂 Dataset

The project uses a **Student Performance Dataset** containing information related to students' academic performance and lifestyle factors.

Examples of variables analyzed include:

* Study Hours
* Attendance Percentage
* Sleep Hours
* Social Media Hours
* Netflix Hours
* Exercise Frequency
* Mental Health Rating
* Exam Score
* Other relevant student-related factors

### Target Variables

**Regression Target:**

```text
exam_score
```

**Classification Target:**

```text
pass_fail
```

Students scoring **50 or above** are considered `Pass`, while students scoring below 50 are considered `Fail`.

---

## 🔎 Exploratory Data Analysis

The following EDA techniques were performed:

### 1. Dataset Inspection

* Dataset shape
* Column names
* Data types
* First few records
* Summary statistics

### 2. Missing Value Analysis

Missing values were identified and handled wherever required.

### 3. Duplicate Analysis

Duplicate records were checked and removed where necessary.

### 4. Numerical and Categorical Variables

The dataset was divided into:

* Numerical variables
* Categorical variables

### 5. Distribution Analysis

Histograms were used to understand the distribution of numerical variables and exam scores.

### 6. Outlier Analysis

Box plots were used to identify potential outliers.

### 7. Correlation Analysis

A correlation heatmap was created to understand relationships between numerical variables.

### 8. Relationship Analysis

Scatter plots were used to analyze relationships between important variables such as:

* Study Hours vs Exam Score
* Attendance vs Exam Score
* Sleep Hours vs Exam Score

---

## 🤖 Machine Learning Workflow

The project follows these major Machine Learning steps:

```text
Data Collection
      ↓
Data Inspection
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Feature Selection
      ↓
Data Preprocessing
      ↓
Train-Test Split
      ↓
Model Training
      ↓
Prediction
      ↓
Model Evaluation
      ↓
Overfitting/Underfitting Analysis
      ↓
Final Insights
```

---

# 📈 Regression Model

## Linear Regression

A **Linear Regression** model was trained to predict students' numerical exam scores.

### Features

Relevant student performance and lifestyle variables were used as input features.

### Target

```text
exam_score
```

### Evaluation Metrics

The following regression metrics were used:

* **Mean Absolute Error (MAE)**
* **Mean Squared Error (MSE)**
* **Root Mean Squared Error (RMSE)**
* **R² Score**

### Interpretation

* **MAE:** Measures the average absolute difference between actual and predicted scores.
* **MSE:** Measures the average squared prediction error.
* **RMSE:** Represents prediction error in the same unit as the target.
* **R² Score:** Indicates how much variation in exam scores is explained by the model.

An actual-vs-predicted scatter plot was also created to visually evaluate the regression model.

---

# ✅ Classification Model

The regression target `exam_score` was converted into a binary classification target.

### Pass/Fail Rule

```text
exam_score >= 50 → Pass
exam_score < 50  → Fail
```

The classification target was encoded as:

```text
1 → Pass
0 → Fail
```

## Logistic Regression

A **Logistic Regression** model was trained to predict whether a student would pass or fail.

### Classification Evaluation Metrics

The model was evaluated using:

* **Accuracy**
* **Precision**
* **Recall**
* **F1-Score**
* **Confusion Matrix**

### Confusion Matrix

The confusion matrix was visualized using a heatmap to understand:

* True Positives
* True Negatives
* False Positives
* False Negatives

---

# 📊 Model Performance Comparison

Training and testing performance was compared for both models.

This comparison helps identify:

### Overfitting

When a model performs very well on training data but significantly worse on testing data.

### Underfitting

When a model performs poorly on both training and testing data.

### Good Generalization

When training and testing performance are reasonably close, indicating that the model generalizes well to unseen data.

---

## 💡 Key Insights

The analysis helps identify important factors associated with student performance, such as:

1. **Study time** can have an important relationship with exam performance.
2. **Attendance** can contribute positively to academic performance.
3. **Sleep patterns** may be associated with students' ability to perform academically.
4. **Lifestyle factors** such as social media usage, entertainment time, and exercise can provide useful information about student performance.
5. **Machine Learning models** can be used to identify performance patterns and predict whether a student is likely to pass or fail.

> The exact strength and direction of these relationships should be interpreted from the actual EDA visualizations and model results obtained in the notebook.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```text
Student-Performance-ML/
│
├── Student_Performance_ML.ipynb
├── Student_Performance.csv
└── README.md
```

---

## ▶️ How to Run the Project

### 1. Clone or download the repository

Download the project files from the repository.

### 2. Open the notebook

Open:

```text
Student_Performance_ML.ipynb
```

using either:

* Jupyter Notebook
* JupyterLab
* Google Colab

### 3. Upload the dataset

Make sure the dataset is available in the notebook environment.

### 4. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 5. Run the notebook

Execute the cells sequentially from data loading to final model evaluation.

---

## 📌 Conclusion

This project demonstrates a complete Machine Learning workflow for analyzing and predicting student performance.

Exploratory Data Analysis was first used to understand the dataset and identify relationships between different student-related factors and exam scores. A Linear Regression model was then developed for predicting numerical exam scores.

The problem was also converted into a classification task by defining a passing threshold of 50 marks. Logistic Regression was used to predict whether a student would pass or fail, and its performance was evaluated using classification metrics and a confusion matrix.

Overall, the project demonstrates how **data analysis and Machine Learning can be combined to understand student performance, identify important factors, and make useful predictions.**

---

## 👩‍💻 Author

**Ritika**

B.Tech Computer Science & Engineering

---

## 📚 Project Type

**Machine Learning | Exploratory Data Analysis | Regression | Classification | Model Evaluation**

**Day 18 & 19 Assignment**
