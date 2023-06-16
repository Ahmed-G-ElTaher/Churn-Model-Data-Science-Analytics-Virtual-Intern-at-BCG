# Data Science & Analytics Virtual Intern at BCG :
 Churn-Model-on-Data-Science-&-Analytics-Virtual-Intern-at-BCG
 
 
 [completion_certificate.pdf](https://github.com/Ahmed-G-ElTaher/Churn-Model-on-Data-Science-and-Analytics-Virtual-Intern-at-BCG/files/11772786/completion_certificate.pdf)

# ______________________________________________________

## - First Task : Business Understanding & Hypothesis Framing
 ### Understanding the business context and problem statement.
#### * PowerCo. needs BCG to help diagnose the source of churning SME customers.
#### * A fair hypothesis is that price changes affect customer churn.
#### * The head of the SME division is considering a 20% discount that is considered large enough to dissuade almost anyone from churning (especially those for whom price is the primary concern).
#### * i email the AD to erquest the data(Customer data,Churn data and Historical price data).
# ______________________________________________________


## - Second Task : Exploratory Data Analysis
 ### Understanding the business through data.
#### * After the AD send the data, i Perform some exploratory data analysis. Look into the data types, data statistics, specific parameters, and variable distributions.
#### * Try to verify the hypothesis of price sensitivity being to some extent correlated with churn.
#### * Try to prepare a half-page summary or slide of key findings and add some suggestions for data augmentation
#### * After EDA, i found some conclusions : 
 - #### on average churned clients drives more gross and net margin 
 - #### consumption and forcasting between two groubs almost the same till 75% 
 - #### net margin will be a little bit higher than the current clients after 20% discount 
# ______________________________________________________
 

## - Third Task : Feature Engineering & Modelling
 ### Uncovering signals within the data, predicting churn probability and evaluating model performance.
 
#### * Sub-Task 1 :
 - #### Think of ways to evaluate a feature against a label.
 - #### Think of ways to add new features which would complement the already existing ones. 
 - #### Think of feature granularity. 
 - #### Remove unnecessary features.
 
#### * Sub-Task 2 :

 - #### Is this problem best represented as classification or regression? 
 - #### What kind of model performance do you think is appropriate? 
 - #### Most importantly how would you measure such a performance? 
 - #### How would you tie business metrics such as profits or savings to the model performance?

#### * After preparing data, i do some feature engineering, then i Start with a Dummy Model (np.rand) - Baseline Model with accuarcy 0.51 and F1_score 0.18
#### * I try a Simple Model (linear) with :
 - #### Linear model
 - #### calculate score
 - #### calculate feature imporance
 - #### Simple model with top 10/20 features
#### * Also i try a Simple Model with Balanced Dataset ( Upsampling[f1-score 0.21], Downsampling[f1-score 0.22] ).
#### * Then i try Complex and Explainable Modeles (Tree Based) :
 - #### Decision Tree (Original_data[f1-score 0.12], Upsampling[f1-score  0.15], Downsampling[f1-score 0.19] ).
 - #### Random Forest (Original_data[f1-score 0.05], Upsampling[f1-score  0.08], Downsampling[f1-score 0.19] ).
#### * Finally i try Deeper Modeles :
 - #### XGBoost (Original_data[f1-score 0.04], Upsampling[f1-score  0.12], Downsampling[f1-score 0.22] ).
 - #### CatBoost (Original_data[f1-score 0.03], Upsampling[f1-score  0.11], Downsampling[f1-score 0.22] ).

#### * The Best Model is : CatBoostClassifier With Downsampling data because the accuracy is higher.


# ______________________________________________________



## - Forth Task : Findings & Recommendations
     Presenting your results and giving recommended actions to the client

