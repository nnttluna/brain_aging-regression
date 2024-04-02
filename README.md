# Model for Brain Aging Prediction

The project aims to develop a computer regression model applied on data of brain features to predict ages, one model from each section, linear, non-linear and trees classification, has been picked to generally present the performance of each class.

# Brain Features Data 

Features such as the thickness and volume of different areas of the human brain were used to determine the age of an individual, ranging from 18 to 96 years. This data set has 4226 instances, and 138
predictors, which are all features taken from a brain MRI scan. This data set was of particular interest to the group, as we all share a common interest in medical imaging along with conditions found in the brain.

Acknowledgements
Data: https://data.mendeley.com/datasets/rscbjbr9sj/2

License: CC BY 4.0

Citation: http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5

# Data Analysis Hypothesis

In comparison on complexity, the Neural Network model is more complicated since it is using the sequential function with 3 high density hidden layers. Since there are 138 predictors, the Neural Network model is presumed to have the best performance among all for the complexity of the dense hidden layers training. Penalized Model is a linear regression model whose algorithm shrinks the regression coefficients toward zero by penalizing the regression model with L1-norm as penalty term, which is the sum of the absolute coefficients. Neural Network Model is non-linear regression method which replicates the actual biological neural network system. There are 128 inputs taken, return 1 output, trained in 3 hidden layers with 256 nodes in each layer. Gradient boosting trees is one of the trees machine learning algorithms for tabular datasets. It is used to find nonlinear relationship between your model target and features and has great usability that can deal with missing values, outliers, and high cardinality categorical variables on your features without any 
special supervision.

# Results

The regression models were applied to 4226 instances in order to predict the age of the
brain. With the R^2 value, it allows for comparing the differences between observed data and a
fitted trend to calculate the dependent variable variation. The highest accuracy model, proved by R2 = 0.9084, is given by 
penalized model, which is a linear regression method. The gradient boosting trees model is 
providing the lowest value of R^2 = 0.8590. However, to prevent overfitting, the model is only 
running with 20 estimators and 2 layers of separation. The model definitely can be improved 
with larger number of estimators and deeper differentiation. 


Overall, these models having the lowest RMSE values meant
that the predicted values were relatively accurate and that these three algorithms were capable
of correctly predicting a subject’s age within a margin of 2.61 years to 7.90 years. As boosted
trees by design function to train low bias estimators in conjunction with an attempt to predict the
error of its preceding learner, this technique proved to be an effective feature for data training.
By contrast, the three models that yielded the worst (ie. the highest) RMSE values were the
decision tree, partial least squares, and bagged models, whose age predictions were inaccurate
by roughly 9.72 to 13.37 years. With the decision tree model having the poorest performance,
this can be explained by its tendency to be sensitive even to a small amount of data variation.
Overall, this suggests that there is some level of instability with this particular model type, as it
lacks boosting or bagging variance handlers.
