# Data-Science-Competitions
## Analytics Vidhya Loan Competition III
##### Loans default will cause huge loss for the banks, so they pay much attention on this issue and apply various method to detect and predict default behaviours of their customers.here I am going to talk about the basic process of loan default prediction with machine learning algorithms.

#Project Motivation::::
The loan is one of the most important products of the banking. All the banks are trying to figure out effective business strategies to persuade customers to apply their loans. However, there are some customers behave negatively after their application are approved. To prevent this situation, banks have to find some methods to predict customers’ behaviours. Machine learning algorithms have a pretty good performance on this purpose, which are widely-used by the banking. Here, I will work on loan behaviours prediction using machine learning models.

#Data Exploration and Preprocessing::::
The data set I use contains several tables with plenty of information about the accounts of the bank customers such as loans, transaction records and credit cards. Here, my main purpose is to predict customer behaviours about loan for each account. Thus, the most important table here is table “loan”. And after checking the description of all the features, we think “order”, “trans” and “card” contain useful info for our purpose. And I also need to use account and disposition to combine them together. Finally, the tables required are highlighted in the following figure.

#Feature Engineering::::
There are some missing values occur in the column “Loan monthly payment”, which means the customers didn’t make payment for their loans. In this situation, the missing values should be imputed with zero instead of mean or median.

#Model Validation and Selection::::
Here I use K-Fold cross validation to split the data without holdout part into training data and validation data and then fit the model. Since the problem is a classification problem, I choose logistic regression, random forest and XG boosting. To compare the performance of these three models, I plot the ROC curve and calculate the AUC score.

#Model Evaluation::::
Now I combine training data and validation data together to fit the random forest and use the holdout testing data set to do the prediction.
