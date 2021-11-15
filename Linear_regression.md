# Linear Regression 

## Linear regression is an algorithm that uses linear approach for modelling the difference between independent and dependent variables.  

## Simple Linear regression is when the model uses one independent variable and Multiple Linear regression is when the model uses more than one independent variables.  

![Simple Linear regression pic](https://cdn-images-1.medium.com/max/1292/1*Nf2tTTkALYq6RTMQmhjo1A.png)

### The equations of a Linear regression line : 

## **Y ₚ = B0 + B1X1 + B₂X₂ + …... + BnXn + ε** 

* Y ₚ = the predicted value of the dependent variable 

* B0 = the y-intercept (value of y when all other parameters are set to 0) 

* B1X1= the regression coefficient (B1) of the first independent variable (X1) (a.k.a. the effect that increasing the value of the independent variable has on the predicted Y ₚ value) 

* … = do the same for however many independent variables you are testing 

* BnXn = the regression coefficient of the last independent variable 

* ε = model error (a.k.a. how much variation there is in our estimate of y) 

## Or **Y ₚ = f(x) + ε** , ie, **Y ₚ = A x + B + ε** 

* f(x) = A x + B 

* A = slope of linear model (dimensional vector of parameters) 

* B = intercept of linear model (real no) 

### We want to find the optimum value of A and B from model data to predict the value of Y ₚ for validation or unknown data.  

### Root mean square error is the Cost function of the linear regression :

## **C = (1/N) ᵢ ₌ ₁ Σ ⁿ (Y ᵢ - f(x ᵢ)) ²**

### (Y ᵢ - f(x ᵢ)) ²² is the loss function and called square loss error.  

### To update A and B values in order to reduce Cost function (minimizing RMSE value) wrt A and B. For achieving the best fit line the model uses Gradient Descent.  

## Initial value of **A (A←0) = ∂C/∂A = (-2/N) ᵢ ₌ ₁ Σ ⁿ (x ᵢY ᵢ)** and  

## Initial value of **B (B←0) = ∂C/∂B = (-2/N) ᵢ ₌ ₁ Σ ⁿ (Y ᵢ)** 

### The idea is to start with initial A and B values and then iteratively updating the values, reaching minimum cost. 

## **A ← A - α(∂C/∂A)**

## **B ← B - α(∂C/∂B)**

### And that’s how we get the values of the variables, if the values are substituted in f(x), we’ll get the linear model for that particular problem. The model will only need value of X features for predicting Y.  
