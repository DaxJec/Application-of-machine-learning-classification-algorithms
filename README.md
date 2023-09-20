# Application-of-machine-learning-classification-algorithms

# Application of the classification algorithms

### Project title : Application scorecard for new customers

#### The scorecard is intended to detect whether the new customer will default (failure to repay a loan installment for more than 90 days)

#### As per the nature of the problem at handle to be solved,this will require building a classfication model.

#### The different classification models are going to be evaluated to identify the one the suits the project. These are;

* Support Vector Machine (SVM)

* Logistic Regression

* KNearestNeighbors

* Decision Tree

* Random forest

#### importing the libraries to used throughout the development of the project

#### Building a fuction that will aid in the load and wrangling of the imported dataframe

##### After importing the data from the provided excel sheet into a pandas dataframe, the following data validation is to be applied.

* Checking the imported dataframe for any null values

* The data types of all the features have to be crossed checked so as to confirm the alignment with the dictionary information

* As the data in the excel sheet was already encoded, we have to confirm the number of unique values in the encoded columns if they match those of the dictionary.

* We have to identify the features to used as the predictive variables and the target feature.

* With "RESPONSE" as the target feature, the rest of the features will be predictive variables

* The observation  (OBS#) feature will have to be dropped out from the predictive features 

#### Preparing the data for building the models

* identifying and defining the target (y) and the predictive features (X); and knowing their shapes

##### The predictive features have to scaled so as to have a mean of zero (0) and standard deviation of one, with help of standard scaler.

##### This synchronizes the scales of the featues. (Using the StandardScaler)

### Building the naive (with default settings) models 

* The models are fitted with the training data

* The performance of the models to be evaluated on both the training and test data

### Applying hyperparameter tuning to obtained the best estimators of the different models.

* the above fitted naive models were performing well however, we need to be prepared for overfitting problem hence hyperparameter tuning

* with the help of the RandomizedSearchCV, we shall tune the various model hyperparameters

* since the data was imbalanced, stratifiedKFold will be used when creating the folds.

* best scores and best parameters for the different tuned models will be captured in a dataframe for evaluation.

### Building the tunned  (with set hyperparameters) models 

* The models are fitted with the training data

* The performance of the models to be evaluated on both the training and test data

### The final model to used for the solving the classification is a Decision Tree.

* the hyperparameters to used are list above.

* at the time of runing this code the parameters were max_features="sqrt",max_depth=11,criterion="gini"

### The final model to used for the solving the classification is a Random forest.

* the hyperparameters to used are list above.

* at the time of runing this code the parameters were n_estimators=150,max_features="log2",max_depth=18,criterion="gini" 'criterion': 'gini
