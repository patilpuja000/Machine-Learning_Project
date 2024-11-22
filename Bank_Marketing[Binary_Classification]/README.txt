Business Objective: The business goal is to find a model that can explain success of a contact, i.e. if the client subscribes the deposit. Such model can increase campaign efficiency 
by identifying the main characteristics that affect success, helping in a better management of the available resources (e.g. human effort, phone calls, time) and selection of a high 
quality and affordable set of potential buying customers. 


Statatic and Interpretation of the analysis :
This is dataset is observed with 2 classes and unbalanced.
In the Cleaning phase , I saw there were no nan values so went ahead with tranforming the categorical features.
For the EDA i considered 2 approches
1. To eliminate all independent features and use only correlated features for first initial round of testing. This excludes duration features even though asked to be considered. 
2. To add some other impotarnat features, this time includes duration fetaure. 
This approach gave a clear understanding on how using different features can improve the models perfomrance as shown in the notebook with model comparsion using hyperparameters. 


Findings from the comparsion and hyperparameters for KNN, Logistic Regression, Decision Tree and SVM.
1. Basemodel perfomance was at 88%
2. Comparing models with default parameters concluded that SVC has better performance score but highly computational, and LogisticRegression/KNN is a better option as it has a 89% 
perfomance testing score.
3. I tried using SMOTE that will create synthetic data for the unbalanced dataset. but the performance is not upto make and can be improved by other methods.
4. Also tried a new model Naive Byes with cumulative gains curve, this did not give a good score for both training and testing.
5. Next attempted for Hyper parameteriazation on  KNN, Logistic Regression, Decision Tree & SVM. KNN with 31 neighbors & logistic regression hyper parmeters gave a best model with
92% Testing score. And Decision tree with Best params: {'criterion': 'gini', 'max_depth': 5, 'min_samples_leaf': 1, 'min_samples_split': 0.05} with atest score of 91%.
SVM has been the highest computational model for simple and hyperparmeters. I could not get the test score for hyperparemeters as my system was crached multiple times. 


Next steps and recommendations : Mentioned in the Notebook
