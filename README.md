# Machine Failure Prediction using Machine Learning - up2246639

## Introduction

This project aims to build a machine learning pipeline to predict whether a machine will fail or not fail.
The dataset contains information about machine operating conditions, including air temperature, process temperature, rotational speed, torque, tool wear, and machine type. The target column used in this project is `Machine failure`.

This is a classification problem because the model predicts one of two possible outcomes:

- `0` = machine does not fail
- `1` = machine fails

## Business objectives

In a real business setting, this type of model could help a company plan maintenance earlier, and avoid unexpected repair costs.

## ML Pipeline

The machine learning pipeline follows these stages:

1.  Data collection

- The dataset was downloaded from Kaggle and saved as: `ai 2020.csv`

- After loading the dataset, several checks were carried out: 
`df.head()`
`df.info()`
`df.isnull().sum()`
`df.duplicated().sum()`
`df.shape`
.These were done to check the structure of the data set, data types and see of there are any missing values or any dupplicate rows

2. EDA

Exploratory Data Analysis was used to understand the dataset before building the machine learning models.

- The target column, Machine failure, was checked using a countplot. This showed that the dataset is imbalanced because there are more machines that did not fail than machines that failed.

- The Type column was also checked to see the distribution of machine types.

- Histograms were created for the numerical features

- Boxplots were created to compare each numerical feature against Machine failure.

- A correlation heatmap was also created to check relationships between numerical features

3. Model building

Two machine learning models were built and compared:

1. Logistic Regression:

This models was selected since its has been designed for classification problems, especially when the target has two classes such as 0 and 1 

2. Random forest Classifier:

Random Forest Classifier was used because it is a strong classification model that combines multiple decision trees to improve prediction performance. 
It can learn more complex patterns in the data compared with a single Decision Tree. 

4. Model evaluation

The models were evaluated using:
- Accuracy score
- Classification report
- Confusion matrix

The initial two model were compared using the validation accuracy score, where the Randomforest model was more accurate. Then after the model optimisation the comparison was carried out again using the validation accuracy score, where the final model was selected as the oppimised Random forest classifier. 

5. Prediction

## Jupyter notebook structure

1. Importing libraries
2. Loading the dataset
3. Data validation checks
4. Exploratory data analysis
5. Feature preparation
6. Training two machine learning models
7. Intial model comparison 
7. Hyperparameter optimisation
8. Final Model comparison
9. Testing on unseen data
10. Conclusion 

## Future work

Future work for the project can include:
 - Testing more modles
 - Using a bigger data set 
 - Using more advanced optimisation for all models 

## Libraries and modules

### pandas

pandas was used to load and handle the dataset.

### matplotlib

matplotlib was used to create visualisations. It was used to control figure sizes, add graph titles, and display plots.

### seaborn

seaborn was used to create clearer statistical graphs. It was used for histograms, boxplots, and correlation heatmaps. 

### scikit-learn
 1. train_test_split 

train_test_split was used to divide the dataset into training, validation, and unseen test sets.

 2. MinMaxScaler 

MinMaxScaler was used to scale the numerical features. This helped place all numerical values on a similar scale before model training.

 3. OneHotEncoder

OneHotEncoder was used to convert categorical text data into numbers so that a machine learning model can use it.

 4. LogisticRegression

LogisticRegression was used as the first classification model.

 5. RandomForestClassifier

 RandomForestClassifier was used as the second classification model

 6. classification_report 

 classification_report was used to show precision, recall, and f1-score.

 7. confusion_matrix 

confusion_matrix was used to show correct and incorrect predictions for each class

## Unfixed bugs

There are no known unfixed bugs in the current version of the notebook.

## Acknowledgements and References

- The dataset used in this project was obtained from Kaggle
- Scikit-learn documentation was used for reserch to improve knowledge  
- AI was used for explanations and provide structure 

## Conclusion

This project successfully created a machine learning pipeline for predicting machine failure.The project included data collection, validation, EDA, data preparation, model building, model evaluation, optimisation, and prediction. 

Two models were trained and compared with eachother, The final model was selected based on validation performance, where Random Forest has achieved the best acuracy. 
Hyperparameter tuning provided improvement in the calidation performance for the random forest. Hence, the improved Random Forest model is selected as the best-performing model.


