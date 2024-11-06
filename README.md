# deep-learning-challenge

# Overview

This project is to build a Neural Network Model for the nonprofit charity group called Alphabet Soup. The goal of this model is to predict the best applicants for funding. Alphabet Soup wants to fund the groups most likely to be successful, and have given a dataset with 34,000 instances of funding to train the data. 

The dataset provided contains these columns:< br/>
-EIN and NAME—Identification columns< br/>
-APPLICATION_TYPE—Alphabet Soup application type< br/>
-AFFILIATION—Affiliated sector of industry< br/>
-CLASSIFICATION—Government organization classification< br/>
-USE_CASE—Use case for funding< br/>
-ORGANIZATION—Organization type< br/>
-STATUS—Active status< br/>
-INCOME_AMT—Income classification< br/>
-SPECIAL_CONSIDERATIONS—Special considerations for application< br/>
-ASK_AMT—Funding amount requested< br/>
-IS_SUCCESSFUL—Was the money used effectively< br/>
< br/>
Using this data, the model was trained using scikit learn and tensorflow. < br/>
< br/>
# Results
-The initial model only achieved a 72% accuracy. 
-The model which performed the best kept the name column and binned the names of 10 or less. 
-Increasing the bin sizes did not increase the accuracy.
-Adding a third hidden layer with 5 perceptrons greatly reduced the accuracy.
< br/>
## Data Processing
The data was first preprocessed. The classification and application type columns were binned to clean up the smaller clumps of data. The target variable for this model was the is successful column. By making this the target, the model will work to predict how successful other funding projects will be in the future. When creating the initial model, the columns EIN and name were removed, as they were deemed not important features of the is successful column (later models show this isn't the case though!). 

## Compiling, Training, and Evaluating the Model
The initial model was trained with 70 neurons in the first layer and 30 in the second. These numbers were chosen because they were suggested by the inital assignment outcomes. With these parameters, the model came up just short of the 75% goal. Changing the number of nodes in both layers did little to change the accuracy.
The optimized models returned very different results. Using the same number of neurons and layers, the model which used binned names instead of deleting the names performed the best. The model wich added a third layer, however, performed the worst of all at less than 50% accuracy. This indicates that names are an important feature to attribute to success when building this model.

# Summary
The end goal was to build a neural network which could predict a successful venture to ensure funding goes to the best oportunity. After optimizing the model, this goal was reached. While the original instructions determined the name column to not be necessary, in the end it was actually very important to the success of the model. 
