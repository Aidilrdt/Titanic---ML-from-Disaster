# Titanic Survival Prediction: Gradient Boosting Model

This repository contains a machine learning project for predicting survival on the Titanic using the Titanic dataset. The model applies a Gradient Boosting Classifier to predict whether a passenger survived or not based on several features like age, sex, class, and more.

## Project Overview

The project uses the Titanic dataset to build a machine learning model capable of predicting passenger survival. The approach involves preprocessing the data, applying feature engineering, and training a Gradient Boosting model. Hyperparameter tuning was also performed to optimize the model's performance.

### Key Features:

- Data Preprocessing: Handle missing values, encode categorical features using One-Hot Encoding.
- Feature Engineering: Added new features like family grouping based on the `Ticket` feature.
- Hyperparameter Tuning: Used Grid Search to optimize the Gradient Boosting model.
- Evaluation: Used accuracy, confusion matrix, and classification report to assess the model.

## Dataset

The dataset used for this project includes the following files:

- `train.csv`: The training dataset used to train the model.
- `test.csv`: The dataset used to test the model after training.

### Key Features:
- **Pclass**: Passenger class (1st, 2nd, or 3rd)
- **Sex**: Gender of the passenger
- **Age**: Age of the passenger
- **Fare**: The fare the passenger paid
- **Title**: The title of the passenger (e.g., Mr, Mrs, etc.)
- **Family and Party Grouping**: Whether the passenger was traveling alone or with a group (based on the `Ticket` feature)
- **Ticket_Prefix**: Prefix derived from the `Ticket` feature
- **Embarked**: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

## Steps

### 1. **Data Preprocessing**:
- Handle missing values in numerical and categorical features using imputation.
- Apply One-Hot Encoding to categorical variables (`Sex`, `Title`, `Family and Party Grouping`, `Ticket_Prefix`, `Embarked`).
- Split the dataset into training and testing sets.

### 2. **Model Training**:
- Train a Gradient Boosting Classifier model using the training set.
- Perform hyperparameter tuning with GridSearchCV to improve model accuracy.

### 3. **Evaluation**:
- Evaluate model performance using accuracy, confusion matrix, and classification report.
- After tuning, evaluate the model's performance on the test set.

### 4. **Results**:
- The Gradient Boosting model achieved an accuracy of **0.8659** on the test set.
