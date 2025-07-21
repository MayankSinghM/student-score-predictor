# Student Marks Prediction

This project predicts a student's score based on the number of hours they studied, using a simple Linear Regression model.

## 📌 Problem Statement

Given the number of hours a student studies, predict the percentage of marks they will score.

## 🔧 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib / Seaborn
- Joblib

## 📊 Dataset

A small dataset with two columns: `Hours` and `Scores`.

| Hours | Scores |
|-------|--------|
| 2.5   | 21     |
| 5.1   | 47     |
| 7.8   | 86     |

## 🧠 Model

- Algorithm: Linear Regression
- Training/Test Split: 80/20
- Evaluation Metric: R² Score

## ✅ Features

- Train a linear regression model
- Save and load the model using `joblib`
- Interactive prediction input
- Visualize the data and regression line

## 📁 How to Run

```python
# Save model
from joblib import dump
dump(model, 'student_score_model.joblib')

# Load model
from joblib import load
model = load('student_score_model.joblib')

# Predict score for 5 hours
model.predict([[5]])
