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

The highest accuracy model, proved by R2 = 0.9084, is given by 
penalized model, which is a linear regression method. The gradient boosting trees model is 
providing the lowest value of R^2 = 0.8590. However, to prevent overfitting, the model is only 
running with 20 estimators and 2 layers of separation. The model definitely can be improved 
with larger number of estimators and deeper differentiation. 

The regression models were applied to 4226 instances in order to predict the age of the
brain. With the R
2 value, it allows for comparing the differences between observed data and a
fitted trend to calculate the dependent variable variation. For the R squared value obtained from
comparing all models, the best results were yielded from the Bagged model, Multiple linear
regression and support vector machine with R
2
, and the worst performing models included
Decision Trees, Partial Least squares, and Neural Network(1). With the top performers being
from different regression methods such as linear regression, non-linear and trees, they all fit the
data observed with R
2 values above 0.8. As for the worst case R
2 models, we observe them to
be less than 0.8 meaning that the points are far from the best fit trend line. All the other models
not discussed within the top 3 and bottom 3 performers yielded results between 0.8 and 0.84
which shows a general regression model that fits the data well with the trend line. Furthermore,
both models from kNN both reproduced similar values within the r^2 table, only differing by 0.01
in R^2 value. On the other hand,an important note to be made is that Neural network(1)
performed at 0.78, Neural Network(2) performed at 0.87, and Neural Network(3) performed at
0.83. This can be explained by differing input numbers varying from 3,128,and 138 as well as
differing hidden layers from 8, 3 and 1 and different number of sized layers used. We found that
better performing models that yielded over 0.8 had more hidden layers than the neural network
model that performed only at 0.78.
As per Figure 3 and Table 2, it can be seen that the three models with the best Root
Mean Square Error (RMSE) results respectively were gradient boosted, random forest trees,
and multiple linear regression. Overall, these models having the lowest RMSE values meant
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
