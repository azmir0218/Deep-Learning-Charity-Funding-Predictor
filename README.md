# Deep Learning: Charity Funding Predictor

## Background

The non-profit foundation Alphabet Soup wants to create an algorithm to predict whether or not applicants for funding will be successful. With our knowledge of machine learning and neural networks, we’ll use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, we have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

* **EIN** and **NAME**—Identification columns
* **APPLICATION_TYPE**—Alphabet Soup application type
* **AFFILIATION**—Affiliated sector of industry
* **CLASSIFICATION**—Government organization classification
* **USE_CASE**—Use case for funding
* **ORGANIZATION**—Organization type
* **STATUS**—Active status
* **INCOME_AMT**—Income classification
* **SPECIAL_CONSIDERATIONS**—Special consideration for application
* **ASK_AMT**—Funding amount requested
* **IS_SUCCESSFUL**—Was the money used effectively

## Instructions

### Step 1: Preprocess the data

Using our knowledge of Pandas and the Scikit-Learn’s `StandardScaler()`, we’ll need to preprocess the dataset in order to compile, train, and evaluate the neural network model later in step 2. 

### Step 2: Compile, Train, and Evaluate the Model

Using our knowledge of TensorFlow, we’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset. we’ll need to think about how many inputs there are before determining the number of neurons and layers in your model. Once we’ve completed that step, we’ll compile, train, and evaluate our binary classification model to calculate the model’s loss and accuracy.

### Step 4: Write a Report on the Neural Network Model

For this part of the Challenge, we’ll write a report on the performance of the deep learning model we created for AlphabetSoup.

The report will contain the following:

1. **Overview** of the analysis: Explaining the purpose of this analysis.

2. **Results**: Addressing the below question

  * Data Preprocessing
    * What variable(s) are considered the target(s) for your model?
    The target variable for this model is "IS SUCCESSFUL" and is denoted by 0 if the result was NO and 1 if YES. 
    * What variable(s) are considered to be the features for your model?
    'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS','ASK_AMT'.
    * What variable(s) are neither targets nor features, and should be removed from the input data?
    EIN and NAME columns were irrelevant and they were removed
  * Compiling, Training, and Evaluating the Model
    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
    This information was changed until the required accuracy for this model was achieved. I started with a higher number of layers and went to smaller number until accuracy was achieved. The ultimate number of layers is 7 and 4
    * Were you able to achieve the target model performance?
    After several attempts I was able to achieve the target model performace. 
    * What steps did you take to try and increase model performance?
    For this assignement I changed the number of layers and data split to 80/20 to get to the 75% accuracy score. 

