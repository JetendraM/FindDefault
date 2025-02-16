# Project Title
Credit Card Fraud Detection

## Overview
This project aims to develop a machine learning model for detecting fraudulent credit card transactions using a dataset of transactions made by European cardholders in September 2013. The dataset is highly imbalanced, with only a small percentage of transactions labeled as fraud.

## Dataset
The dataset contains transactions made in two days, with 492 frauds out of 284,807 transactions. The positive class (frauds) accounts for 0.172% of all transactions. The dataset file is named `credit_card.csv`.An highly imbalanced dataset.

## Code and Resources Used
Python Version: Jupyter notebook
Packages: pandas, matplotlib, seaborn, numpy, sklearn, imblearn

## Project Detail

EDA :
- Checked for the null values in the dataset.
- Checked the imbalance in Class in the dataset.
- How the fraud and the non-fraudulent  occurs with respect to the transaction amount and distribution of the amount for positive(frauds) and negative(non-fraudulent) is 
  shown in   a graph.
- Distribution of time also analysed as it doesnot largely affect the dataset.

Data Preprocessing :
- The imbalance in data can be handled by many methods, I have tried with both undersampling and oversampling but good gooed results in oversampling using SMOTE.
- After applying SMOTE the imbalnce in the data is handled by oversampling the positive class(frauds) with the same as negative class(non-frauds)

Model Training :
The machine learning model used for this project is a LogisticRegression, DecisionTreeClassifier, KNeighborsClassifier, RandomForestClassifier and XGBClassifier. Adjustments to hyperparameters and model evaluation metrics are discussed in the notebook. Got good results in RandomForestClassifier model.

## Results 

The model achieved the following results on the test set,
   Accuracy:   0.999918238308078
   Precision:  0.9998363993310551
   Recall:     1.0
   F1 score:   0.9999181929736854

## Conclusion

  SMOTE solves the imbalance in the dataset by oversampling.
  The model Random Forest Classifier applied to this dataset gives almost perfect accuracy for the dataset.







