# Project-
Predictive Maintanance Using Machine Learning 

Introduction: 

Brief description of the project (ca. 10 lines in markdown format)

Business objectives:

State a purpose of the project and project goal. E.g. set the target for prediction probability

ML Pipeline:

 ML Pipeline must tell the story. In our case, the story begins when you acquire out dataset
and finishes when you test our model using data previously unseen by the model

1. Data collection

 Describe here how you collect the data. Provide code snippets (if necessary)



 Describe here how you check and validate the data (e.g. checking correct data format)
 Describe here how you split the dataset into training/validation/test subsets

2. EDA

 Document how you explore the dataset (what it is made of, label distribution, is it balanced?
etc.)

3. Model building

 Document how you choose and build your model. Explain and justify selection of this
particular model type, starting hyperparameters and their optimisation, etc.

4. Model evaluation

 Document model evaluation. Use appropriate error metrics. Model building will, the most
likely, be an iterative process. You might want to optimise hyperparameters and model
architecture, change training process to improve model generalisation, reduce overfitting
and loss. Describe model training curves here.

5. Prediction

 Document testing model in predicting previously unseen dataset and individual input.
Include representative examples.

Jupyter notebook structure:

 Describe structure of Jupyter Notebook

Future work:

 Describe your ideas - what could you improve in this project provided more time is given

Libraries and modules:

### pandas

`pandas` is used for loading the CSV file, storing the dataset as a dataframe, checking column types, summarising values, and creating prediction result tables. It is also used for selecting features and separating the target variable from the input variables.

### numpy

`numpy` is used for numerical operations and array handling. It supports the numerical processing behind the machine learning workflow and is useful when working with model outputs such as prediction probabilities.

### matplotlib

`matplotlib` is used to create visualisations such as bar charts, boxplots, confusion matrix plots, and ROC curves. These graphs help explain the dataset and model performance clearly.

### seaborn

`seaborn` is used for more readable statistical visualisations, including count plots, correlation heatmaps, and boxplots. It improves the presentation of EDA outputs and helps identify relationships between variables.

### scikit-learn

`scikit-learn` is the main machine learning library used in this project. It provides tools for train/test splitting, preprocessing, model pipelines, model training, hyperparameter tuning, predictions, and evaluation metrics.


 Give a list of used Python libraries and modules with brief description (ca. 5 lines of
markdown text each) what they do, what they are for and how they were used

Unfixed bugs:

Acknowledgements and References:

 You must mention if (and where) you used ChatGPT or reused snippets of code from other
people
 Include references if external resources were used to help with your work.

Conclusions: