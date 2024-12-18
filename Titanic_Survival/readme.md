# Titanic Survival Prediction

## Overview
This project uses machine learning techniques to predict the survival of passengers aboard the Titanic based on various features like class, sex, age, and family relations. The goal is to build a model that predicts whether a passenger survived or not based on the available features in the dataset.

## Data
The dataset used in this project consists of the Titanic dataset, which is publicly available on Kaggle. It contains the following columns:

- **PassengerId**: Unique identifier for each passenger
- **Pclass**: Passenger class (1, 2, 3)
- **Name**: Name of the passenger
- **Sex**: Gender of the passenger
- **Age**: Age of the passenger
- **SibSp**: Number of siblings/spouses aboard the Titanic
- **Parch**: Number of parents/children aboard the Titanic
- **Ticket**: Ticket number
- **Fare**: Amount paid for the ticket
- **Cabin**: Cabin number
- **Embarked**: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

The target variable is `Survived`, where:
- `0` represents the passenger did not survive.
- `1` represents the passenger survived.

## Project Workflow

1. **Data Preprocessing**:
   - Handle missing values in features such as `Age`, `Cabin`, and `Embarked`.
   - Convert categorical features (e.g., `Sex`, `Embarked`) into numeric values using one-hot encoding.
   - Split the data into training and testing sets.

2. **Model Selection**:
   The following models are used to predict survival:
   - **Random Forest Classifier**
   - **Logistic Regression**
   - **Decision Tree Classifier**
   - **Support Vector Machine (SVM)**
   - **Gradient Boosting**

   The performance of each model is evaluated using **Accuracy** and **F1 Score** metrics.

3. **Model Training**:
   - Each model is trained using the training data.
   - The model's performance is evaluated on the training set to calculate the accuracy and F1 score.

4. **Prediction**:
   - Each model predicts whether a passenger survived or not in the test dataset.
   - The predictions are displayed along with the corresponding `PassengerId`.

## Installation

To run this project, you need to have Python 3.x installed along with the necessary libraries. Follow the steps below to set up your environment:

### 1. Clone the repository:
```bash
git clone https://github.com/noureldinmo/Classification_models/titanic-survival-prediction.git
cd titanic-survival-prediction

