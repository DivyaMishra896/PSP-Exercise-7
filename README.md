### README.md

# User Behavior Analysis: Logistic Regression, KNN, and Linear Regression

This project demonstrates the use of **Logistic Regression**, **K-Nearest Neighbors (KNN)**, and **Linear Regression** to analyze user behavior data. It includes data preprocessing, model training, predictions, and visualization of results using Python.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Dependencies](#dependencies)
4. [Code Details](#code-details)
   - [Logistic Regression](#logistic-regression)
   - [K-Nearest Neighbors (KNN)](#k-nearest-neighbors-knn)
   - [Linear Regression](#linear-regression)
5. [Visualizations](#visualizations)
6. [How to Run](#how-to-run)
7. [License](#license)

---

## Project Overview

This project uses a dataset containing user behavior metrics such as app usage time, screen-on time, battery drain, and more to predict behavior classes and app usage trends.  
The techniques implemented include:

- **Logistic Regression** for classification.
- **K-Nearest Neighbors (KNN)** for classification.
- **Linear Regression** for predicting app usage time.

The project also generates five different visualizations for better insight into the data and model performance.

---

## Dataset

The dataset (`user_behavior_dataset.csv`) contains the following columns:

- **User ID:** Unique identifier for each user.
- **Device Model:** Type of device.
- **Operating System:** OS used by the device.
- **App Usage Time (min/day):** Total time spent using apps.
- **Screen On Time (hours/day):** Total time the screen was on.
- **Battery Drain (mAh/day):** Daily battery consumption.
- **Number of Apps Installed:** Total installed apps.
- **Data Usage (MB/day):** Total data usage per day.
- **Age:** User's age.
- **Gender:** User's gender.
- **Behavior Class:** Target variable indicating user behavior type.

---

## Dependencies

Install the required Python packages before running the code:

```bash
pip install pandas numpy matplotlib scikit-learn
```

---

## Code Details

### Logistic Regression

- **Task:** Classify user behavior using metrics like app usage time, screen-on time, and battery drain.
- **Output:** 
  - Predicted user behavior classes.
  - **Confusion Matrix Plot:** A heatmap visualization of the model's performance.

### K-Nearest Neighbors (KNN)

- **Task:** Classify user behavior and evaluate the effect of varying the number of neighbors (K).
- **Output:** 
  - Accuracy scores for different values of K.
  - **Accuracy vs. Number of Neighbors Plot:** A line graph showing the impact of K on model accuracy.

### Linear Regression

- **Task:** Predict app usage time based on battery drain.
- **Output:**
  - Predicted app usage times.
  - **Actual vs. Predicted Values Plot:** Scatterplot comparing predictions to actual values.
  - **Residuals Histogram:** Distribution of prediction errors (residuals).

---

## Visualizations

1. **Confusion Matrix for Logistic Regression**
   - Visualizes true vs. predicted labels for behavior classification.

2. **Accuracy vs. Number of Neighbors for KNN**
   - Shows how the choice of K impacts model accuracy.

3. **Actual vs. Predicted App Usage for Linear Regression**
   - Compares true app usage times to model predictions.

4. **Residuals Histogram for Linear Regression**
   - Displays the distribution of prediction errors.

---

## How to Run

1. Place the `user_behavior_dataset.csv` file in the same directory as the code.
2. Run the script using Python:

   ```bash
   python script_name.py
   ```

3. The script will:
   - Print dataset correlation and column details.
   - Train Logistic Regression, KNN, and Linear Regression models.
   - Generate visualizations for each model.

4. View the generated plots for insights.

---

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code with appropriate attribution.

---
