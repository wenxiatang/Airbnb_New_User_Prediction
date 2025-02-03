This is a kaggle competition for [Airbnb New User Prediction](https://www.kaggle.com/competitions/airbnb-recruiting-new-user-bookings). 
# Business Problem
Airbnb wants to predict the first destination a new user would book. By accurately predicting where a new user will book their first travel experience, Airbnb can share more personalized content with their community, decrease the average time to first booking, and better forecast demand.
# Define it as an ML problem
This is a multiclass classification problem. A user can choose from 10 destinations. We want to predict the most probable 5 destinations. 
# Dataset 
train_users_2: Information on 213,451 covering 16 features, such as gender, age, signup_method, language, etc.
test_users: Information on 62,096 covering 15 features same as in train_users_2, excluding target country_destination. 
sessions: data on user sessions, such as action, action_type, and action_detail. Each user has several rows of data. Only 135,483 users have this data. 
countries: general information on 10 destinations. 
ag_gender_bkts: general information on males in 10 groups choosing Australia as a destination. 
# Performance Metrics
I use negative log loss for this classification problem. 
# EDA 
I implement initial data visualization and perform univariate and variate analysis. 
# Feature Engineering
I create new features based on existing features and prepare the data for modeling. 
# Modeling
I have used three models: logistic regression, random forest, XGboost, and Naive Bayes. The best model is a random forest. 
Heatmap of m_estimators and max_depth for CV: 
![CV Heatmap]("C:\Users\Wenxia\Desktop\Python\Airbnb_prediction\data\test_heatmap.png")

