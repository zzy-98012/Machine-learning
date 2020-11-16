# Machine Learning and Transportation
## Project1: Buston Housing Prediction

1.Data  
We used two different sets of data to predict the prices of Buston Housing.The first one which has 489 data points with 4 variables each comes with the project.The name is housing.csv.The other which has 506 data points with 14 variables each comes from the textbook.The name is housing.data.

2.Methods  
We use three methods of Regression which had been listed below:SVR,KNeighborsRegressor,GradientBoostingRegressor.From the textbook's explanation,these three methods are quite accurate in predicting the result.

2.1 The process of coding  
At the beginnning,We import and read the index of the housing price comes from the projects.And we can use 'data.head()' and 'data.info()' to check whether the data were read correctly.Then,with the module of 'train_test_split', 25% of the data was used for testing, and the remaining 75% was used to build the training set.Also,the 'random_state' can be set to whatever value you want.But diffirent values have diffierent degrees of influence on the predicted results. With the module of StandardScaler,the standardization of data reduces the error caused by large difference of data.

From sklearn.svm,sklearn.neighbors,sklearn.ensemble GradientBoostingRegressor.The system will use mathematical models to train the data and  make predictions.Certainly,some models like SVR have various parameters which are different kinds of kernel function such as  'poly', 'linear', 'rbf', etc.We have used the second set of data to compare the predictions of these three kinds of kernel.

Finally,I evaluated the predicted results on value of number,including two measures of R_Squared,MAE,MSE.Because of the same value,I can use both measures of R_Squared.When I use the model of SVR,no matter what the kernel is,the R2_score are always negative.The result of SVR is quite different from those of the other two methods.We can see it visually in the diagram.

2.2 graph  
  There are two graphs to showu the results.One is to show the difference of three methods,the other is to show which is the best kernel between 'linear','poly','rbf' when I use the method of SVR.Graph1 is a histogram and Graph2 is a linechart. THe contrast is all clear.  
<img src="image/picture1.png" height="500" width="450">


3.Some questions I can't deal  
  When I standardized the data with the the module of StandardScaler,I can only standardize the 'X_train' and 'X_test'.If I standardized the 'y_train' and 'y_test',there were some questions I can't find.Therefore, my results are quite different from those in the book when compare the difference of various kernel for SVR.
