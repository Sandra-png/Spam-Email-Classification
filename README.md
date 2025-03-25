# Spam Email Classification

This project involved building a machine learning model to classify emails as either spam or legitimate using Naive Bayes. The project started by conducting a data cleaning and exploratory data analysis (EDA). I then measured the performance of the model using metrics like accuracy, precision, recall, F1 score, confusion matrice.

## Dataset
https://www.kaggle.com/datasets/balaka18/email-spam-classification-dataset-csv

## Key Features
### Cleaning the Dataset
- Imported and cleaned the dataset by checking for and removing missing values and duplicates.
- Conducted an EDA using descriptive statistics and visualizations to understand the feature distributions and class imbalance.

### Feature Engineering
- Removed non-informative columns like "Email No."
- Defined features (X) and target (y)
- Split the data into training and teseting sets, using an 80/20 split

### Modeling
- Used Multinominal Naive Bayes classifier
- Trained the model on the training set
- Evaluated its performance on the test set

## Model Evaluation
  - Accuracy: 95.46%
  - Precision: 89%
  - Recall: 95.95%
  - F1 Score: 92.36%
