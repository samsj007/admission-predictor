# 🎓 AI Admission Predictor

## 📌 Project Overview

**AI Admission Predictor** is a Machine Learning-based web application designed to predict the expected number of student admissions for a college.

The application uses **7 important admission-related factors** as input and applies a trained **Random Forest Regression** model to estimate the number of students likely to be admitted.

The prediction is displayed through an easy-to-use web interface along with visual charts for better understanding of **admission levels and seat utilisation**.

> **Note:** The model is trained using a generated practice dataset. Therefore, the predictions are intended for demonstration and decision-support purposes and are not guaranteed real-world forecasts.

## 🎯 Objectives

* Predict the expected number of college admissions.
* Analyze multiple factors affecting admissions.
* Compare Machine Learning regression models.
* Provide a simple web interface for prediction.
* Visualize prediction results using charts.
* Support college planning for seats, staff, and facilities.

## 📊 Input Features

The model uses the following **7 factors**:

1. **Applications Received**
2. **Seats Available**
3. **Placement Percentage**
4. **Advertisement Budget**
5. **Courses Available**
6. **Annual Fees**
7. **Last Year's Admissions**

## 🤖 Machine Learning Model

Two regression algorithms were evaluated:

| Model                        |       MAE |  R² Score |
| ---------------------------- | --------: | --------: |
| Linear Regression            |     88.33 |     0.619 |
| **Random Forest Regression** | **56.97** | **0.820** |

Based on the practice dataset, **Random Forest Regression** performed better than Linear Regression.

### Why Random Forest?

Random Forest combines multiple decision trees to make predictions. It can capture relationships between multiple factors more effectively than a simple linear relationship.

## ⚙️ How It Works

```text
User enters 7 factors
        ↓
Web Form
        ↓
Flask Backend
        ↓
Input Validation
        ↓
Random Forest Model
        ↓
Admission Prediction
        ↓
Seat Capacity Check
        ↓
Charts & Results
```

The predicted admission count is capped at the available seats because a college cannot admit more students than its sanctioned seat capacity.

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Scikit-learn**
* **Flask**
* **HTML**
* **CSS**
* **JavaScript**
* **Chart.js**
* **Git & GitHub**
* **Render**

## 📈 Model Evaluation

### MAE – Mean Absolute Error

MAE represents the average difference between the predicted and actual values.

**Lower MAE indicates better performance.**

### R² Score

R² indicates how much of the variation in the target variable is explained by the model.

**A value closer to 1 generally indicates better performance.**

## 📊 Visualization

The application provides visual representations of the prediction, including:

* **Admission Prediction Bar Chart**
* **Seat Utilisation Doughnut Chart**

These visualizations make the prediction easier to understand.

## 🌐 Application Architecture

```text
Frontend
   │
   ▼
Flask API
   │
   ▼
Machine Learning Model
   │
   ▼
Random Forest Regression
   │
   ▼
Predicted Admissions
   │
   ▼
Chart.js Visualization
```

## ⚠️ Limitations

* The model uses a generated practice dataset.
* Real-world prediction accuracy has not been established.
* Only 7 factors are currently considered.
* The project does not currently use a production database.
* Real admission decisions may depend on additional factors not included in the model.

## 🔮 Future Enhancements

* Train the model using real multi-year college admission data.
* Add more relevant admission factors.
* Provide course-wise admission predictions.
* Add historical admission trend analysis.
* Integrate a database.
* Add user authentication.
* Display model performance metrics within the application.
* Improve prediction accuracy using larger real-world datasets.

## 🚀 Deployment

The application can be deployed using **Render** with the source code maintained in GitHub.

```text
GitHub Repository
       ↓
     Render
       ↓
Public Web Application
```

## 📌 Disclaimer

This project is intended for **educational, demonstration, and decision-support purposes**. The dataset used for training is generated practice data, so the predicted admission numbers should not be treated as guaranteed real-world values.

---

### ⭐ AI Admission Predictor

**Machine Learning-powered admission forecasting for smarter college planning.**
