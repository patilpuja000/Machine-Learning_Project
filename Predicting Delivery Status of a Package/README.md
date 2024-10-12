### Project Title
Predicting Delivery Status for a Shipment by estimating the Shipment Delays[FedEx]

**Author**
Pooja Patil 
Email : poopat350@gmail.com


#### Executive summary

#### Rationale & #### Research Question
(Why should anyone care about this question and What are you trying to answer )

-> Research Description : 
In today’s fast-paced world, efficient delivery and logistics are crucial for businesses. Predicting delivery times accurately and estimating shipment delays can help companies 
streamline their operations, optimize resources, and provide better customer service. Machine learning techniques can be employed to analyze historical data and build predictive 
models that can forecast delivery times and identify potential delays.

I will consider one such example dataset from FedEx logictics company. Here, Business has to evaluate a lot of factors before taking a decision to deliver a package. The objective 
of this project is to optimize the process of planning delivery.

Predicting delivery time and estimating shipment delays with machine learning can be a valuable tool for businesses in the logistics industry. It allows them to make data-driven 
decisions, optimize their operations, and provide better service to their customers.To address this I am working on this project which will maximize the security of deliveries and
minimize dissappointments of lost.

-> Goal : 
Before diving into the implementation, let’s understand the problem we are trying to solve. Our goal is to predict the delivery status for shipments and by estimating potential 
delays and compare with the Planned_Delivery_Time based on historical data from 2008. We will use machine learning algorithms to train a model that can learn from past deliveries 
and make predictions on new, unseen data. The analysis also include other features to predict the delivery_status.


#### Data Sources
-> Gathering and Preparing the Data
To build our predictive model, we have a dataset that includes information about past deliveries, such as shipment details, timestamps, and actual delivery times and dependent 
variable called as Delivery_status(0 indicates delivered on time and 1 indicates not delivered).
The reason for not delivered can be anything some examples are Lack of visiblity, Delyaed Deliveries, Lost of Stolen Packages, Wrong Delivery Address, Damaged Packages etc. 

The data for this project can be obtained from publicly available datasets, website Kraggle : https://www.kaggle.com/datasets/vasudevmaduri/fedexdata/data

Once we have collected the data, we need to preprocess and prepare it for the machine learning model. This involves tasks such as handling missing values, encoding categorical 
variables, and scaling numerical features. Python libraries such as Pandas and Scikit-learn are excellent tools for data preprocessing.


#### Methodology
-> Exploratory Data Analysis (EDA)
EDA is a crucial step in any data analysis project. It helps us understand the structure and patterns present in the data. During EDA, we can perform tasks such as visualizing 
the distribution of features, identifying outliers, and examining relationships between variables. Matplotlib, Plotly and Seaborn are popular Python libraries for data 
visualization.

-> Feature Engineering
Feature engineering involves creating new features or transforming existing ones to enhance the predictive power of our model. In the context of delivery time prediction, 
we can extract useful information from the existing features, such as the day of the week, hour of the day, or distance between the origin and destination. Feature engineering 
requires domain knowledge and creativity to capture relevant information that can improve the model’s performance.Since I have previously worked on a Pickup and Delivery 
operations project under FedEx i have tried to use the appropriate features for the model predictions.


-> Splitting the Data
Before building our machine learning model, we need to split the dataset into training and testing sets. The training set will be used to train the model, while the testing set 
will be used to evaluate its performance on unseen data. The Scikit-learn library provides convenient functions to split the data into training and testing sets.


-> Building the Machine Learning Model
Now it's time to build our machine learning model. As this research focuses on the status 0 or 1 which indicates classification. Hence ,I will be working with several classiication 
algorithms such as Logistic Regression, k-Nearest Neighbors , Decision Trees along with cross validation and hyperparameters. Next will use the strongest models like Random Forest 
,XGBoost and AdaBoost to check the accuracies.Each algorithm has its strengths and weaknesses,and the choice depends on the specific problem and dataset. I will not consider 
Support Vector Machine becasue this dataset is huge and SVM is not efficient working with huge data.

As this dataset is unbalanced i will be using SMOTE to make the target variable balanced for better model performance.The Scikit-learn library provides implementations of various 
classification models. However, after some research a way to undersample the target variable is possible by using imbalanced learn class's RandomUnderSampler function  imporve 
the perfomance of the model and I will use the undersample approach.

I have also tried to train the model bt using simple neural network with relu activation for binary crossentropy. 

#### Results
-> Model Evaluation
After training our model, we need to evaluate its performance to ensure its effectiveness. Common evaluation metrics for classification tasks include Accuracy, Presicion,
Recall, F1-Score, ROC Curve and AUC. We can use these metrics to assess how well our model predicts the delivery status and estimate the potential delays.


-> Predicting Delivery Time and Estimating Shipment Delays (Test Data)
Once we have built and evaluated our model, we can use it to make predictions on new, unseen data. Given a set of features for a shipment, our model can predict the delivery 
status and estimate potential delays.


#### Next steps
This can greatly assist businesses in optimizing their operations and providing better customer service.We have to continuously iterate and improve this model by experimenting 
with different algorithms, feature engineering techniques, and evaluation metrics.

#### Outline of project

- [Link to notebook 1]()


##### Contact and Further Information
Email : poopat350@gmail.com

