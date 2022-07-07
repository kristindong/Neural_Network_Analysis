# Neural Network Charity Analysis

## Overview

This is a binary classification problem using neural networks and deep learning algorithms to predict if applicants for a charity funding will be successful. 

The dataset used to train and test the model contains more than 34,000 organizations that have received funding over the years, and includes information about the organizations such as type and funding amounts, and whether the organization was successful after being funded.

## Results

Deliverable 1: Preprocessing Data for a Neural Network Model
Deliverable 2: Compile, Train, and Evaluate the Model
Deliverable 3: Optimize the Model
Deliverable 4: A Written Report on the Neural Network Model (README.md)


### Data Preprocessing

Target:
- IS_SUCCESSFUL (1 = yes / 0 = no)

Features:
- APPLICATION_TYPE           
- AFFILIATION                  
- CLASSIFICATION              
- USE_CASE                     
- ORGANIZATION                 
- STATUS                       
- INCOME_AMT                   
- SPECIAL_CONSIDERATIONS       
- ASK_AMT                  

Variables that do not contribute to the model and were removed:
- EIN
- NAME

### Compiling, Training, and Evaluating the Model

Initially, the following 2-layer neural network was used. Since it's a binary classification problem, a Sigmoid activstion function was used for the output layer. This model did not achieve the target accuracy of 75%.



To imcrease model performance, the following modifications were made:
1. adjusted the grouping of rare occurances of CLASSIFICATION to allow for more distinct groups, i.e., more granularity
2. increased the number neurson from 8 to 24 in layer one, and from 5 to 10 neurons in layer two
3. added a thrid ReLU hidden layer with 10 neurons
4. increased the number of epochs from 100 to 200

However, these modifications did not meaningfully increase model performance, and the model's accuracy is still below 75%.

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.




