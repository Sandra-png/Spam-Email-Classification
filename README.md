# Spam Email Classification

This project involved building a machine learning model to classify emails as either spam or legitimate using Naive Bayes. The project started by conducting a data cleaning and exploratory data analysis (EDA). I then measured the performance of the model using metrics like accuracy, precision, recall, F1 score, confusion matrice.

## Why Naive Bayes?
The supervised learning classification algorithm for spam detection that I chose for this was Naive Bayes. Naive Bayes is commonly used in spam filtering. In this case, Naive Bayes would calculate the probability of each class given its data points, and will then choose the class with the highest probability. Naive Bayes is an especially good at text classifications, and can handle the high quantity of text emails can produce, and therefore seems like the correct choice for this task. Specifically the Multinominal Naive Bayes classifier.

In the next code snippets I am preparing the data by dropping the "Email No." and "Prediction" columns, with the target variable being the "Prediction" column. The model learns that the Y predicted spam emails have "z" features from X, and from the correlation can predict spam emails.

I thereafter split the dataset into training and testing, where 20% goes into testing after training.

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
