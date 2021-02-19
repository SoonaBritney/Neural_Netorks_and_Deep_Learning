# Neural_Netorks_and_Deep_Learning

### Technology:Neural networks and Deep Learning
### Data: 

## Challenge Overview
We received a CSV containing more than 34,000 organizations that have received various amounts of funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

## Objectives
#### 1. Deliverable 1: Preprocessing Data for a Neural Network Model
- The following preprocessing steps have been performed:
  - The EIN and NAME columns have been dropped (5 pt)
  - The columns with more than 10 unique values have been grouped together (5 pt)
  - The categorical variables have been encoded using one-hot encoding (5 pt)
  - The preprocessed data is split into features and target arrays (5 pt)
  - The preprocessed data is split into training and testing datasets (5 pt)
  - The numerical values have been standardized using the StandardScaler() module (5 pt)
#### 2. Deliverable 2: Compile, Train, and Evaluate the Model
- The neural network model using Tensorflow Keras contains working code that performs the following steps:
  - The number of layers, the number of neurons per layer, and activation function are defined (2.5 pt)
  - An output layer with an activation function is created (2.5 pt)
  - There is an output for the structure of the model (5 pt)
  - There is an output of the model’s loss and accuracy (5 pt)
  - The model's weights are saved every 5 epochs (2.5 pt)
  - The results are saved to an HDF5 file (2.5 pt)
#### 3. Deliverable 3: Optimize the Model
- Using your knowledge of TensorFlow, optimize your model in order to achieve a target predictive accuracy higher than 75%. If you can't achieve an accuracy higher than 75%, you'll need to make at least three attempts to do so.
#### 4. Deliverable 4: A Written Report on the Neural Network Model (README.md)
- Overview of the analysis: Explain the purpose of this analysis.
- Results: Using bulleted lists and images to support your answers, address the following questions.
  - Data Preprocessing
  - What variable(s) are considered the target(s) for your model?
  - What variable(s) are considered to be the features for your model?
  - What variable(s) are neither targets nor features, and should be removed from the input data?
  - Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - Were you able to achieve the target model performance?
  - What steps did you take to try and increase model performance?

### Summary / Conclusion

1). How many neurons and layers did you select for your neural network model? Why?
For the input layer, I added the number of input features equal to the number of variables in the feature DataFrame.
In the hidden layers I added two hidden layers with only a few neurons in each layer. To create the second hidden layer, I added another Keras Dense class while defining our model.
All of our hidden layers will use the relu activation function to identify nonlinear characteristics from the input values.
In the output layer, I used the same parameters from our basic neural network including the sigmoid activation function. 
The sigmoid activation function will help us predict whether or not an applicant will be successful if funded by Alphabet Soup.

2). Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
Looking at our deep learning model’s performance metrics, the model was able to correctly identify applicants who will be successful if funded by Alphabet Soup approximately 73% of the time. 
The deep learning model was able to produce a fairly reliable classifier. 
I tried doubling the epochs from 100 to 200. When compared to the previous deep learning model, this model produced a less reliable classifier. 
This models accuracy was 0.7254810333251953, while the previous model was 0.7271137237548828

3) If you were to implement a different model to solve this classification problem, which would you choose? Why?
I would us a Random forest classifier. 
Random forest classifiers are a type of ensemble learning model that combines multiple smaller models into a more robust and accurate model. 
They use a number of weak learner algorithms and combine their output to make a final classification decision. 
Random forest models have been popular in machine learning algorithms for many years due to their robustness and scalability. 
Both output and feature selection of random forest models are easy to interpret, and they can easily handle outliers and nonlinear data.
