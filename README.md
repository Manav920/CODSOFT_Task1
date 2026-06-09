# Titanic Survival Prediction

## Project Overview

This project is about using computers to guess if someone survived the disaster. We look at things like how old they were if they were a man or woman what class ticket they had, how much they paid for the ticket and details about their family.

The goal is to make a model that says:

* **1** → They survived

* **0** → They did not survive

## Dataset

We use a list of people who were on the Titanic. The list has things like:

* What class they were in (Pclass)

* If they were a man or woman (Sex)

* How old they were (Age)

* How much they paid for their ticket (Fare)

* How brothers or sisters they had with them (SibSp)

* How parents or kids they had with them (Parch)

* Where they got on the boat (Embarked Port)

* If they survived (which we are trying to guess)

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

We load the list into our computer using Pandas. We then look at the list to see what it has. If there are any missing pieces of information.

### 2. Exploratory Data Analysis (EDA)

We do some digging to understand the list:

* We look at a summary of the list

* We see how many people survived

* We see how much people paid across classes

* We make some charts to see how things are related

### 3. Data Cleaning

We clean up the list:

* We get rid of things we don't need:

* PassengerId

* Cabin

* Name

* Ticket

* We fix missing information:

* Age → We use the age

* Embarked → We use the common place

### 4. Feature Engineering

We make the list better for our model:

* We change the Fare so its not too skewed

* We turn things like Sex. Embarked into numbers

We change:

* Sex

* Embarked

### 5. Feature Selection

We separate the list into:

* The things we use to make a guess (X)

* What we are trying to guess (y = Survived)

### 6. Model Training

We use a tool called a Random Forest Classifier to make our guesses.

We split our list into:

* 75% for training

* 25% for testing

### 7. Model Evaluation

We see how good our model is by seeing how often it gets it right.

**We got it right 82.8% of the time**

## Results

Our model is pretty good, at guessing if someone survived. It gets it right about **82.8% of the time**. This shows that cleaning up the list and making it better really helped.
