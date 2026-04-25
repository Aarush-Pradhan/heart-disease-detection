# Heart Disease Detection Using Machine Learning

## Project Overview

This project aims to predict whether a person is likely to have heart disease based on medical attributes using Machine Learning algorithms. The system analyzes patient health parameters and classifies the result as:

* **0 → No Heart Disease**
* **1 → Heart Disease Present**

This is a **Binary Classification Problem** in Machine Learning.

---

## Problem Statement

Heart disease is one of the major causes of death worldwide. Early detection can help in timely treatment and reduce serious health risks.

The goal of this project is to build a Machine Learning model that can predict the presence of heart disease using patient medical data.

---

## Dataset Used

The project uses the **Heart Disease UCI Dataset** (commonly available on Kaggle and UCI Repository).

### Features Used

| Feature  | Description                                   |
| -------- | --------------------------------------------- |
| age      | Age of the patient                            |
| sex      | Gender (1 = Male, 0 = Female)                 |
| cp       | Chest pain type                               |
| trestbps | Resting blood pressure                        |
| chol     | Serum cholesterol                             |
| fbs      | Fasting blood sugar                           |
| restecg  | Resting electrocardiographic results          |
| thalach  | Maximum heart rate achieved                   |
| exang    | Exercise-induced angina                       |
| oldpeak  | ST depression induced by exercise             |
| slope    | Slope of peak exercise ST segment             |
| ca       | Number of major vessels                       |
| thal     | Thalassemia                                   |
| target   | Output variable (1 = Disease, 0 = No Disease) |

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Collection

* Loaded the Heart Disease dataset from CSV format

### 2. Data Preprocessing

* Checked missing values
* Removed duplicate records
* Verified data consistency

### 3. Exploratory Data Analysis (EDA)

Performed:

* Correlation Heatmap
* Feature Relationship Analysis
* Target Distribution Check

Important features identified:

* cp
* thalach
* exang
* oldpeak
* ca
* thal
* slope

### 4. Train-Test Split

Dataset was divided into:

* 80% Training Data
* 20% Testing Data

Using:

* `random_state = 42`
* `stratify = target`

### 5. Feature Scaling

Applied **StandardScaler** before Logistic Regression to improve convergence and model performance.

### 6. Model Training

Implemented:

* Logistic Regression
* Random Forest Classifier

### 7. Model Evaluation

Evaluated using:

* Accuracy Score
* Confusion Matrix
* Classification Report

### 8. Model Comparison

Compared both models and selected the best-performing model.

---

## Models Used

### Logistic Regression

Used as the baseline classification model.

### Random Forest Classifier

Used for improved prediction and comparison.

---

## Results

| Model               | Accuracy |
| ------------------- | -------: |
| Logistic Regression |81.967213%|
| Random Forest       |78.688525%|



### Best Model Selected

Based on evaluation, the better-performing model was selected for final prediction.

---

## Confusion Matrix

Used to evaluate:

* True Positive
* True Negative
* False Positive
* False Negative

This helps understand model performance beyond accuracy.

---

## Conclusion

Heart Disease Detection was successfully performed using Machine Learning techniques.

After comparing Logistic Regression and Random Forest models, the project identified the most effective model for prediction.

Features like chest pain type (`cp`), exercise-induced angina (`exang`), maximum heart rate (`thalach`), and oldpeak showed strong influence on prediction.

This project demonstrates how Machine Learning can support early disease detection and improve healthcare decision-making.

---

## Future Improvements

Possible future enhancements:

* Hyperparameter tuning for better accuracy
* Model deployment using Flask or Streamlit
* Real-time prediction system using user input
* Integration with hospital management systems

---

## Author

Aarush Pradhan

B.Tech Student
Machine Learning Project
Heart Disease Detection System
