# Soft Introduction to Machine Learning

2023-02-26

## What is Machine Learning?

Machine learning is a branch of computer science which aims to develope algorithms and *models* that enable a computer to learn intrinsic information from data and make predictions.

<br>

This is in stark contrast to just logic based algorithms which can be modeled as rules which once written don't change and cannot learn from new information or data available. Much of traditional softwares that has been written over the past decades since the advent of modern computing has been logic based programs. They have helped humans efficiently perform tasks from simple calculations to putting people on the moon. Although they have made life simple and can do advanced computation they have not been able to magically learn from data.

<br>

The idea of machine learning algorithms is not new and has been present since decades but it was during the 1950s when they were first developed. One of the earliest algorithms was developed in 1957/58 by Frank Rosenblatt. The [Perceptron][@1] is a type of artificial neural network that can learn to classify input data into one of two categories. Similarly [*Recurrent Neural Networks(RNN)*][@2] was proposed during the 80s and [*Long Short-Term Memory(LSTMs)*][@3] during the late 90s. But at that time the computation power available was not sufficient to actually make these algorithms work in a feasible manner.

<br>

## Common Machine Learning Tasks

The tasks for machine learning has change drastically over the last couple of years especially with the advent of *Neural Networks*.


The most common tasks today for machine learning can be categorized as follow - 

1. Classification: This involves identifying which category or class a given input data. For example, determining whether a picture is of cat or dog.

2. Regression: This involves predicting a numerical value based on input data. For example, predicting the price of a house based on its features like square footage, number of bedrooms, etc.

3. Clustering: This involves grouping similar data points together based on their similarities. For example, grouping similar people according to their spending habits.

4. Dimensionality Reduction: This involves reducing the number of features in a dataset while retaining as much information as possible. For example, reducing the number of features in an image dataset while retaining as much information as possible.

5. Recommendation Systems: This involves recommending items to users based on their past behavior. For example, recommending movies to users based on their past movie-watching history.

6. Natural Language Processing (NLP): This involves processing and understanding human language, including tasks such as text classification, sentiment analysis, and language translation. 

7. Audio: This category like the previous one has a lot of sub-tasks which can be listed like - audio synthesis, audio recognition etc. 

Although we have put forward 7 categories as of writing this article, I am sure more tasks will be needed to be classified as we explore more in the field. 

Another thing of note is that the tasks above are not strict categories, meaning one task can be modelled as another. For example, a classification problem can be modelled as regression probelem and vice-versa given the features allow that transformation of the problem. 

<br>

## Quick Overview of Terms 

<br>

### Features 
Features are input variables or attributes which represent the data being analyzed. Broadly there are two types - categorical and numerical but there can be much for complex features like images, time-series, text, audio etc.

<br>

### Model
The model is the output of the learned representation of the algorithm on the data it was trained on. Think of it as the output of a training on the input dataset. The model once trained can be used for prediction for the task it was trained on. For instance if we were training a model to predict house prices based on input features like zipcode, rooms, area etc, once the model is trained and we feed it a unseen feature set (of the same features) it should be accurately able to tell you what the house price should be. 

<br>

### Training 
Training refers to the process of putting the input dataset into the ML algorithm for it the *learn* about the intrinsic parameters of the dataset. 

<br>

### Parameter
Parameters are the internal settings or weights of a model that are learned during the training process. This is something that the model learns from the data and not to be confused with hyper-parameters. The goal of the ML  practitioner is to find the best algorithm which can be used to learn the intrinsic *parameters* of the data which will help them to accurately predict the target when it is given a new feature set.

<br>

### Hyperparameters
This is the external settings which is under the control of the practitioner. This changes with the algorithm being used for example for a Linear Regression model might include - learning rate, number of iterations, regularization etc. 

### Target
Target refers to what we are trying to predict from the task at hand. For example - house prices, stock prices, type of image etc. 


<br>

## Final Thoughts
We are in a very exciting time in our history to be witnessing the rapid growth of machine learning and its uses. It would be a shame for one to not have a basic understanding of ML and how we can leverage it to benefit ourselves and in large our society enabling us to all grow together. 

## Reference
[@1]:https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.335.3398&rep=rep1&type=pdf
[@2]:https://apps.dtic.mil/dtic/tr/fulltext/u2/a164453.pdf
[@3]:https://deeplearning.cs.cmu.edu/S23/document/readings/LSTM.pdf