# Titanic Survival Prediction

## Project Overview

This project uses Machine Learning to predict whether a passenger survived the Titanic disaster based on passenger information such as age, gender, ticket class, fare, and family details.

The objective is to build a binary classification model that predicts:

* **1** → Survived
* **0** → Did Not Survive

## Dataset

The project uses the famous Titanic dataset containing passenger information including:

* Passenger Class (Pclass)
* Sex
* Age
* Fare
* Number of Siblings/Spouses (SibSp)
* Number of Parents/Children (Parch)
* Embarked Port
* Survival Status (Target Variable)

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

## Project Workflow

### 1. Data Loading

The Titanic dataset is loaded using Pandas and inspected for structure and missing values.

### 2. Exploratory Data Analysis (EDA)

Performed various analyses to understand the dataset:

* Dataset information summary
* Survival distribution analysis
* Fare distribution across passenger classes
* Statistical summaries using pivot tables
* Correlation analysis using heatmaps

### 3. Data Cleaning

The following preprocessing steps were performed:

* Removed unnecessary columns:

  * PassengerId
  * Cabin
  * Name
  * Ticket

* Handled missing values:

  * Age → Filled using mean value
  * Embarked → Filled using mode value

### 4. Feature Engineering

To improve model performance:

* Applied logarithmic transformation to the Fare feature to reduce skewness.
* Converted categorical variables into numerical form using Label Encoding.

Encoded columns:

* Sex
* Embarked

### 5. Feature Selection

Features and target variable were separated:

* Features (X)
* Target (y = Survived)

### 6. Model Training

A Random Forest Classifier was used for prediction.

The dataset was split into:

* 75% Training Data
* 25% Testing Data

### 7. Model Evaluation

Model performance was evaluated using classification accuracy.

**Achieved Accuracy: ~82.8%**

## Results

The Random Forest model successfully predicts passenger survival with approximately **82.8% accuracy**, demonstrating the effectiveness of data preprocessing and feature engineering techniques.

##

##
