# Ev Fiyat Tahmini
It is a house price prediction project based on a boston house-pricing dataset and used Linear Regression for Machine Learning Algorithm. 
A lot of libraries are used in this project. You can check them out down below.
# NumPy:
- NumPy is the fundamental package for scientific computing in Python. 
It is a Python library that provides a multidimensional array object, 
various derived objects (such as masked arrays and matrices), and an assortment of 
routines for fast operations on arrays, including mathematical, logical, 
shape manipulation, sorting, selecting, I/O, discrete Fourier transforms, 
basic linear algebra, basic statistical operations, random simulation and much more.
 
   ![image](https://user-images.githubusercontent.com/55557233/143553382-407c9754-edba-456d-aa34-47daf385a14d.png)
# Pandas:
- Pandas is a Python library used for working with data sets.
  It has functions for analyzing, cleaning, exploring, and manipulating data.
  Pandas allows us to analyze big data and make conclusions based on statistical theories.
  Pandas can clean messy data sets, and make them readable and relevant.
 
   ![image](https://miro.medium.com/max/481/1*cxfqR8NAj8HGal8CVOZ7hg.png)
    
# Scikit-learn:
 - Scikit-learn is a free software machine learning 
   library for the Python programming language. It features various classification, regression and 
   clustering algorithms including support vector machines, random forests, gradient boosting, 
   k-means and DBSCAN, and is designed to interoperate with the Python numerical and scientific libraries NumPy and SciPy.
 
   ![image](https://i2.wp.com/cdn.analyticsvidhya.com/wp-content/uploads/2021/07/31648feature-image-edit.png?resize=350%2C200&ssl=1)
   
# Matplotlib and Seaborn:
 - The most commonly used data visualization tools in python for data science and machine learning.
 
   ![image](https://blueorange.digital/wp-content/uploads/2019/12/Logo_Seaborn.png)
   ![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQofaLU1xF_18T5qp53gWmPwKfuOvAsOB3Vka1DUMLZ6FCNSDpR-U0T37S35bEc_-jd48g&usqp=CAU)
   
# Abstract:
At first we started by searching for a house prices dataset. And we found a Boston House-Pricing dataset on kaggle(link down below).

It has 14 attributes, 13 for prediction, 1 for the price itself. Each record in the dataset describes a Boston suburb or town. 
The data was drawn from the Boston Standard Metropolitan Statistical Area (SMSA) in 1970. And it was pre-processed for machine learning algorithms.

So we did not manipulate the dataset. Since we were going to make a price prediction(which is a number) we used a regression algorithm. 

Cause this problem was a regression problem. We did think about XGBoost Regressor(which is one of the high-end algorithms for regression), 
but it was very complicated and hard to understand for us so we have decided on a basic regression algorithm, which is Linear Regression.

We got the dataset from kaggle and loaded it into a pandas dataframe, split it into X and Y. X is for first 13 attributes, Y is for the last attribute(price).

After that we applied cross validation by splitting dataset into two parts; %75 for the train and %25 for the test.
And we have set the model for our project to Linear Regression from the Scikit-learn library. 

We have fitted it and got 0.7375 R^2 score for train and 0.7313 for the test.
And also we got 3.15 mean absolute error for train, 3.63 for the test.

And we have also checked whether there is a overfitting or underfitting situation by visualizing the predictions and actual values. 
For that we have used Matplotlib library, compared the prediction prices and actual prices. And it seemed fine. 

At the end of the project we have a model for house price prediction
with an accuracy score of %85(There is no exact accuracy score for regression problems so it is an approximate percentage) and 3.63 mean absolute error for test values.

- Kaggle Dataset Link: https://www.kaggle.com/prasadperera/the-boston-housing-dataset/data?select=housing.csv
