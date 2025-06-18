# ml-marketing-campaign
The provided dataset contains ~411k records related with marketing campaign run by bank to attract consumers for term
depposit with lucrative interest rate. Contacts campaign data mainly comprise of first and final contact data however, only the numbers of intermediate contacts with prospective customer to be retained rather then the complete feature data. 

# Summary of the findings/actions
- Null values
  - No null values present
- 'Unknown' Values
  - 'Unknown' values present under 'job', 'marital', 'education', 'default', 'housing' & 'loan' features only
  - All records with 'unknown' features eliminated which is ~0.03% of total records _i.e. 10,700_ exist in dataset
- Reformat columns with _Captialization_ & remove _unknown characters_
- Scaled social indexes _employment variation rate_, _consumer price index_, _consumer confidence index_, & 
  _euribor 3 month rate_ & _number of employees_ based on median

**Observation**
- Higher number of customers with job '_Admins_' contacted. _Admin_ being the highest % turn-out among 
  the categories who subscribed for term deposit
- Higher number of _Student_ (__50.8%__) has subscribed for Term Deposits thought total population % 
  student seleceted to offer deposits   very low  
- __41.5%__ '_Retired_' population selected to be contacted has opted
- __20.5%__ '_Unemployed_' has opted to subscribe for Term Deposit
- Higher number of customers contacted by telecomminication are '_Admin_' and about __16%__ of contacted 
  are converted which in terms of total number is highest 
- Surprisingly, turn-out rate for '_Blue-collar_' jobs are 8% only
- Order of turn-outs in % of the contact population based on _Marital Status_ is __Married > single > Divorces__
- 2 extremes of the educations - '_Univesity Degree_ (__14.8%__) ' & '_Basic 4Y_ (__13.69%__)' group subscribe 
  to term deposit in higher %
- Based on % customers subscribed : __'Univesity Degree' > 'Basic 4Y' > 'Professional Degree' > 'High School'__
- Not many _defaulters_ to be part of cleaned data set
- Turn out rate is better for contacts having higher call duration 
- Successful contacts only when call duration is > 100 min
- '_May_','_July_', '_Aug_' '_June_' are the best months for turn-out for customer contacts, _May_ being the best
  for month to be contacted for turn-out

**Modeling Objectives**
- Compare the performance of the classifiers :
  - K Nearest Neighbor
  - Logistic Regression
  - Decision Trees
  - Support Vector Machines
- Based on parameters :
  - Time to fit
  - Predication efficacy

**Modeling**
- Run all the classifier algorithms - KNN, Logistic regression, Decision Tree and SVM, with default hyperparameters
  ![Model Performance - Before] (/images/Model Performance - After.png)
- Execute cross validation with chosen hyper-parameters for different Algorithms respectively
- Model with the best estimators in individual classifiers 
  ![Model Performance - After] (/images/Model Performance - Before.png)

**Recommandations** :
- Further analysis is needed to segment blue collar segment to increase the turn-around which usually have higher
  value customer to attrect or invest in research for new term deposit plan/options
- '_Retired_' population is more attracted to term deposits, more contacts and increase population may increase the 
  turn-out rate
- Increase contact points with prospective customers in the month of '_May_' & '_July'

# Link to Jupyter notebook
[notebook link](https://github.com/vishalnigam/ml-marketing-campaign/blob/main/ml-maeketing-campaign.ipynb)