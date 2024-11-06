# deep-learning-challenge

# Overview

This project is to build a Neural Network Model for the nonprofit charity group called Alphabet Soup. The goal of this model is to predict the best applicants for funding. Alphabet Soup wants to fund the groups most likely to be successful, and have given a dataset with 34,000 instances of funding to train the data. 

The dataset provided contains these columns:
  -EIN and NAME—Identification columns
  -APPLICATION_TYPE—Alphabet Soup application type
  -AFFILIATION—Affiliated sector of industry
  -CLASSIFICATION—Government organization classification
  -USE_CASE—Use case for funding
  -ORGANIZATION—Organization type
  -STATUS—Active status
  -INCOME_AMT—Income classification
  -SPECIAL_CONSIDERATIONS—Special considerations for application
  -ASK_AMT—Funding amount requested
  -IS_SUCCESSFUL—Was the money used effectively

Using this data, the model was trained using scikit learn and tensorflow. 

# Creating the Model
The data was first preprocessed. The classification and application type columns were binned to clean up the smaller clumps of data. The target variable for this model was the is successful column. By making this the target, the model will work to predict how successful other funding projects will be in the future. When creating the initial model, the columns EIN and name were removed, as they were deemed not important features of the is successful column (later models dispute this thinking though!). 
