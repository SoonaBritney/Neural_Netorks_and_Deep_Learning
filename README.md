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
#### Deliverable 1: Preprocessing Data for a Neural Network Model
#### Deliverable 2: Compile, Train, and Evaluate the Model
#### Deliverable 3: Optimize the Model
- Using your knowledge of TensorFlow, optimize your model in order to achieve a target predictive accuracy higher than 75%. If you can't achieve an accuracy higher than 75%, you'll need to make at least three attempts to do so.
#### Deliverable 4: A Written Report on the Neural Network Model (README.md)


Import and characterize the input data.

What variable(s) are considered the target for your model?
What variable(s) are considered to be the features for your model?
What variable(s) are neither and should be removed from the input data?
Preprocess all numerical and categorical variables.

Combine rare categorical values via bucketing.
Encode categorical variables using one-hot encoding.
Standardize numerical variables using TensorFlow’s StandardScaler class.
Using a TensorFlow neural network design, create a binary classification model that can predict if an Alphabet Soup funded organization will be successful based on the features in the dataset.

Compile, train, and evaluate our binary classification model.

Final model loss metric
Final model predictive accuracy
Optimize our model training and input data to achieve a target predictive accuracy higher than 75%.

Create a new README.txt file within the same folder as our AlphabetSoupChallenge.ipynb notebook.

### Conclusion
How many neurons and layers did you select for your neural network model? Why?
Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
If you were to implement a different model to solve this classification problem, which would you choose? Why?

How many neurons and layers did you select for your neural network model? Why?
For the input layer, I added the number of input features equal to the number of variables in the feature DataFrame.
In the hidden layers I added two hidden layers with only a few neurons in each layer. To create the second hidden layer, I added another Keras Dense class while defining our model.
All of our hidden layers will use the relu activation function to identify nonlinear characteristics from the input values.
In the output layer, I used the same parameters from our basic neural network including the sigmoid activation function. 
The sigmoid activation function will help us predict whether or not an applicant will be successful if funded by Alphabet Soup.

Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
Looking at our deep learning model’s performance metrics, the model was able to correctly identify applicants who will be successful if funded by Alphabet Soup approximately 73% of the time. 
The deep learning model was able to produce a fairly reliable classifier. 
I tried doubling the epochs from 100 to 200. When compared to the previous deep learning model, this model produced a less reliable classifier. 
This models accuracy was 0.7254810333251953, while the previous model was 0.7271137237548828

If you were to implement a different model to solve this classification problem, which would you choose? Why?
I would us a Random forest classifier. 
Random forest classifiers are a type of ensemble learning model that combines multiple smaller models into a more robust and accurate model. 
They use a number of weak learner algorithms and combine their output to make a final classification decision. 
Random forest models have been popular in machine learning algorithms for many years due to their robustness and scalability. 
Both output and feature selection of random forest models are easy to interpret, and they can easily handle outliers and nonlinear data.
