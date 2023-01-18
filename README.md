# sarah_portfolio.github.io

## [Project 1 : Credit-Card-Fraud-Detection-Under-Extreme-Imbalanced-Data : Project Overview](https://github.com/sarahsobri/Credit-Card-Fraud-Detection-Under-Extreme-Imbalanced-Data)

##### Due to the small number of cases of one class, the machine learning model struggles to generalise the behaviour of the minority class, resulting in poor predicted accuracy (Japkowicz & Stephen, 1998). This has hampered the ability of numerous models to function to their full capacity in tackling this long-standing issue. As a result, multiple resampling approaches will be used in this project, including:

1. Random under-sampling
2. Synthetic Modified Oversampling Technique (SMOTE) 
3. Modified Synthetic Modified Oversampling Technique (MSMOTE) 

##### The outcome of these machine learning models have been assessed by their:
1. Sensitivity 
2. Specificity
3. Accuracy
4. Precision
5. Recall
6. F1-Score

##### The classification techniques which were used to classify the resampled datasets were:
1. Logistic Regression
2. Random Forest
3. XGBoost

### Data Source and Type

##### This project makes use of a standard dataset that is freely available on Kaggle, where it comprises over 284,807 records of credit card transactions of European cardholders that occurred within two days in September 2013. The dataset is highly imbalanced where it displays only 492 fraudulent transactions out of 284,807 transactions.

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Imbalanced%20dataset.png)

### Exploratory Data Analysis
#### Library Used

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/EDA.png)

##### Skimpy is a lightweight programme that also offers summary statistics for datagram variables.There are 284807 rows and 31 columns, as we can see. No data is missing.   

![]([https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/EDA.png](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Descriptive%20Analysis.png)

#### Removing Duplicates

##### The dataset contains no null values by default. However, it contained 1081 duplicate values. 

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Remove%20duplicates.png)

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Data%20summary%20after%20removing%20duplicates.png)

##### Using the skim function to remove the duplicated values, we discovered that the dataset now has 283726 rows. We also discovered that the non-fraud class now has 283253 rows while the fraud class had 473 rows.

#### Standardization 

##### Rescaling the range of data so that the mean of observed data is 0 and the standard deviation is 1 is the process of standardising a dataset.The fit transform() method alters the data points while also fitting and transforming the input data. It calculates the mean and standard deviation at the same time as it changes the variable's data points. Because their values differed substantially from the others, we just need to scale the 'Time' and 'Amount' variables.

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Standardisation.png)

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Standardisation%202.png)

#### Feature Engineering

##### The time column gives very little valuable insight because we do not have a launch time for the first transaction. As a result, we have added a new column called 'Time Hour' to the dataset and removed the previous 'Time' feature.

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Feature%20Engineering.png)

#### Data Splitting

##### We have given x the task of carrying all the independent variables and y the task of carrying only the target variable, 'Class.' The data was then split into x train, x test, y train, and y test using the train_test_split function, with the training set receiving 80% of the data and the test set receiving the remainder.

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Data%20Splitting.png)

#### Result Summary

##### Upon completeing the analysis, we have found that the best model that outperforms the rest with the best-balanced trade-off is the random forest with SMOTE with precision of 88% and recall of approximately 85%. Morever, the model achieved an overall accuracy of approximately 100%. 

![](https://github.com/sarahsobri/sarah_portfolio.github.io/blob/main/images/Final%20Result.png)






