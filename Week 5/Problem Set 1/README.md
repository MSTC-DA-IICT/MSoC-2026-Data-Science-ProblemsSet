# MSoC Week Assignment: Car Price Prediction using Linear Regression

## Objective

Build a machine learning model to predict the selling price of a car using Linear Regression. The goal of this assignment is to understand the complete machine learning workflow, including data loading, preprocessing, visualization, model training, and evaluation.

---

## Dataset

Dataset: Car Price Prediction Dataset

---

## Tasks

### Task 1: Load the Dataset

* Download the dataset from Kaggle.
* Load the dataset using Pandas.
* Display:

  * First 5 rows
  * Last 5 rows
  * Shape of the dataset
  * Column names
  * Data types

---

### Task 2: Explore the Dataset

Perform basic data exploration:

* Use `df.info()`
* Use `df.describe()`
* Find the number of missing values.
* Find duplicate rows.
* Remove duplicates if present.

---

### Task 3: Data Cleaning

* Handle missing values.
* Convert categorical columns into numerical values.
* Check for invalid or inconsistent data.
* Prepare the dataset for machine learning.

---

### Task 4: Data Visualization (Matplotlib)

Create the following visualizations:

1. Histogram of car prices.
2. Scatter plot:

   * Mileage vs Price
   * Year vs Price
3. Bar chart of fuel types.
4. Correlation heatmap.
5. Box plot to detect outliers.

All plots must be created using Matplotlib.

---

### Task 5: Feature Selection

Select appropriate input features (X) and target variable (y).

Split the dataset into:

* Training set (80%)
* Testing set (20%)

---

### Task 6: Build a Linear Regression Model

* Import Linear Regression from Scikit-Learn.
* Train the model.
* Make predictions on the test set.

---

### Task 7: Model Evaluation

Calculate the following metrics:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

Interpret the results.

---

### Task 8: Prediction

Take one sample car from the dataset and predict its selling price using your trained model.

---

## Bonus Tasks

1. Compare Linear Regression with Decision Tree Regression.
2. Identify the most important features.
3. Perform feature scaling and compare results.
4. Try removing outliers and observe the change in performance.

---

## Submission Requirements

Submit:

1. Jupyter Notebook (.ipynb)
2. Python file (.py)
