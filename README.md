# Neural Network Charity Analysis

## Overview

The purpose of this analysis was to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup and where to make investments. Alphabet Soup’s business team received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.

Deliverable 1: Preprocessing Data for a Neural Network Model

Deliverable 2: Compile, Train, and Evaluate the Model

Deliverable 3: Optimize the Model

## Resources 

 -Data Source: charity_data.csv
 
 -Data Software and Tools: Python, Anaconda, Jupyter Notebook and Pandas
 
## Analysis and Results of Data

**Data Preprocessing**

*What variable(s) are considered the target(s) for your model?
   The dataset was preprocessed by identifying the value of variables, dropping unecessary columns, binning when possible, and encoding bins to binary values.

*What variable(s) are considered to be the features for your model?
  Target variable: IS_SUCCESSFUL
  Feature variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

*What variable(s) are neither targets nor features, and should be removed from the input data?
  Removed variables: EIN, NAME

**Compiling, Training, and Evaluating the Model**

*How many neurons, layers, and activation functions did you select for your neural network model, and why?

The dataset was split into training and testing data and fitted with a standard scaler by using IS_SUCCESSFUL as the feature value. After many attempts adjusting the number of neurons on each node layer, to keep from overfitting is outlined below: 

![Neural_Nodes](https://user-images.githubusercontent.com/108022219/198419537-d388564a-0501-4a0e-b937-5aea53c883fa.png)

*Were you able to achieve the target model performance?

This resulted consistently in a 72% accuracy level for the testing data:

![D1_Accuracy](https://user-images.githubusercontent.com/108022219/198419881-8ce9a006-0eae-4a39-a830-53bfcac23ad4.png)

What steps did you take to try and increase model performance?
By examining the dataset and attempting to determine if dropping any other non-important variables might lessen the margin of error. Further optimization attempts were made by adding neurons, hidden layers, and altering the activation functions of those layers.  


## Summary 
 
