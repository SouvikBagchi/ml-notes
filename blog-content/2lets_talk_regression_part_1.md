# Let's talk Regression - Part 1

## What is Regression?
Regression is one of the most fundamental tasks of machine learning. It is form of *supervised learning* where the goal is to predict *continuous numerical* output based on one or more input variables. The input variables are called features. 

The goal of a regression model is to learn the relationship between the input variables and the output variable by analyzing the training data and finding the best-fit line or curve that represents the relationship.

<br/>

## Simple Linear Regression 

The most basic case of regression where you are trying to fit a line is called simple regression. As the name suggests - simple meaning in one dimension, linear as in a line and regression as in trying to regress to a value. 

The line equation can be represented by the simeple equation - 

```
y = mx + c
```

The job of the model you are training would be to figure out the values of `m` and `c` where the values of *x* and *y* is the data you would get from the training data. 

Consider the image below - 

![Cat](https://github.com/SouvikBagchi/ml-notes/blob/main/blog-content/images/2_lets_talk_regression/lr1.png?raw=true)


We can tell that if we were to try to fit a line it should be one where most of the points are close to the line as shown below - 

![Cat](https://github.com/SouvikBagchi/ml-notes/blob/main/blog-content/images/2_lets_talk_regression/lr2.png?raw=true)

This is the most simple form of regression in one dimension. 

Say the line equation came out to be - 

```
y = 0.001x + 0.8
```

Now we can easily predict the values of *y* given an input feature *x*.
If we were given an input feature *x* with a value of 500 then substituting the values in the equation we will get the value of 1.3 as shown below:

```
y = 0.001*500 + 0.8
y = 0.5 + 0.8
y = 1.3
```


<br>

## Multinomial Regression
Multinomial regression is taking simple regression and increasing the number of dimensions which corresponds to having more than one feature variables. 

Here the equation of the line we are trying to fit becomes - 



y = &beta;<sub>0</sub>x + &beta;<sub>1</sub>x<sub>1</sub> + ... + &beta;<sub>n</sub>x<sub>n</sub> 

<br>

It's good to visualize how dimensions would look like so I've included the image below - 


![Cat](https://github.com/SouvikBagchi/ml-notes/blob/main/blog-content/images/2_lets_talk_regression/lr34.jpeg?raw=true)

There are three dimensions here *x*, *y* and *z* and the yellow dots represent the data points. The yellow solid line is the regression line that was formed in the feature space(there are three features).

Similarly one can imagine higher dimensions where the model will try to fit the the data points with a single line. 

<br>

## Tasks where Linear Regression is Used

Some of the most common tasks for using regression are as follows - 

* House prices: Linear regression can be used to predict the sale price of a house based on features like its lot size, number of bedrooms, location etc. 

* Sales forecasting: It can be used to predict future sales for a business based on past sales data and other features like marketing expenditure, seasonality, and economic indicators.

* Customer Churn Prediction: Linear regression can be used to predict the likelihood that a customer will churn or leave a business based on features like their purchase history, demographics etc.

* Credit Scores: Linear regression can be used to predict the creditworthiness of a borrower based on their credit history, income etc. 

* Medical diagnosis: Linear regression can be used to predict the likelihood of a disease based on patient characteristics such as age, gender, medical history etc. 

<br>

## Strengths 
One of the major strengths of linear regression is that all of the parameters learned can be easily viewed. This means the model is very easily explained and tweaking the features and seeing the parameters change is extremely valuable to certain types of business. For instance in case of loan lending using a linear regression model can be very useful given we can see if there is bias by looking at the parameters and seeing what the weights are given to which features. 

<br>

## Drawbacks
The major drawback of linear regression is that it always tries to fit a line. So it is not handy in trying to learn a function which is in higher order. This poses problems where the model cannot generalize more complex decision boundaries and will only somewhat try to approximate to a line.

We will explore this in more details in the coming posts. 

<br>

## Takeaways

Regression is a form of supervised learning to predict continuous numerical output given input feature variables. 

The most basic forms of regressions are simple linear regression and polynomial regression. 

Although linear regression can be used for a lot of ML tasks and is easily explainable it doesn't generalize well to tasks where the function can be more complex. 

Despite the drawbacks, linear regression is a very powerful tool and worth learning as a first step towards your machine learning journey. 