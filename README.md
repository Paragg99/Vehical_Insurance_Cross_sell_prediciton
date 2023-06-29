# Health_Insurance_Cross_sell_prediciton

Predict Health Insurance Owners' who will be interested in Vehicle Insurance

## Problem Statement

Your client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the customers from past year will also be interested in Vehicle Insurance provided by the company.

## Business Goal

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

## Data Discription

Data Source : Kaggle

Data Source Link : https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction?select=train.csv

The Dataset used for the analysis includes the following columns:

id : Unique ID for the customer

Gender : Gender of the customer

Age : Age of the customer

Driving_License : 0 - Customer does not have DL,1 - Customer already has DL

Region_Code : Unique code for the region of the customer

Previously_Insured : 1 - Customer already has Vehicle Insurance, 0-Customer doesn't have Vehicle Insurance

Vehicle_Age : Age of the Vehicle Vehicle_Damage : 1 - Customer got his/her vehicle damaged in the past. 0 -Customer didn't get his/her vehicle damaged in the past.

Annual_Premium : The amount customer needs to pay as premium in the year

PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.

Vintage : Number of Days, Customer has been associated with the company

Response : 1 - Customer is interested, 0 - Customer is not interested

## Model Building

To build the insurance sales prediction classification model, the following steps were performed:

**Data Overview :**
An overview of the dataset was conducted to understand its structure and characteristics. The dataset consists of historical data on insurance customers, including features such as age, gender, annual_premium, vehical_age, vehical_damage, previous purchase, and driving_lisence. The dataset was examined for the number of instances, features, data types, and any missing values.

**Exploratory Data Analysis (EDA) :**
EDA was performed to gain insights into the relationships between variables and uncover patterns or trends in the data. Statistical analysis and summary statistics were calculated, and the distribution of each feature was explored. Correlations between features and the target variable were identified to determine their relevance for the prediction task.

**Data Visualization :**
Data visualization techniques were used to provide a clear representation of the data and reveal important insights. Plots such as histograms, scatter plots, box plots, and correlation matrices were created to visualize the relationships and distributions of the features. These visualizations helped in identifying outliers, class imbalances, and potential feature transformations.

**Feature Engineering :**
Feature engineering techniques were applied to improve the predictive power of the model. This involved creating new features or transforming existing ones. Categorical variables were one-hot encoded, interaction terms were created, and new features were derived from existing ones. These feature engineering steps aimed to capture additional information and improve the model's performance.

**Feature Scaling :**
To ensure that all features are on a similar scale, feature scaling was performed. This step is important, especially for algorithms that are sensitive to the scale of the input features. Common scaling techniques include standardization (mean normalization) and normalization (min-max scaling). The chosen scaling method depends on the specific requirements of the models being used.

**Model Selection :**
Two classification models, Random Forest Classifier and XGBoost Classifier, were selected for building the insurance sales prediction model. These models were chosen based on their performance in similar prediction tasks and their accuracy and all accuray matirx evaluation. Model selection involved evaluating different algorithms and choosing the ones that provided the best performance metrics.

**Model Building with Hyperparameter Tuning :**
The selected models, Random Forest Classifier and XGBoost Classifier, were built with hyperparameter tuning. Hyperparameters are configuration settings that determine the behavior of the models during the training process. By tuning these hyperparameters, the models can be optimized for better performance. Techniques such as grid search, random search, or Bayesian optimization were employed to find the best combination of hyperparameters for each model.

## Conclusion

The ML model for the problem statement was created using python with the help of the dataset, and the ML model created with Random Forest and XGBClassifier models performed better than Logistics Regression model with 89% accuracy. Thus, for the given problem, the models created by Random Forest and XGBClassifier.
