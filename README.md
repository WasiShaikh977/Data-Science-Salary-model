# Data-Science-Salary-model
### Project Overview
- Created a model that estimates the salary for a job in data (data science,data analysis,MLE, etc)
- Exploratory analysis of the data to find patterns and get insights
- Visualisation of the said patterns and insights
- Tested on Linear, Lasso and Random Forest Regressor. Used GridSearchCV to optimize our best model

![](https://github.com/WasiShaikh977/Data-Science-Salary-model/blob/main/salary.png)

### Resources
**Python Version:** 3.11


**Packages:** pandas, matplotlib, seaborn, numpy, sklearn, wordcloudm nltk


**Tutorial:** [https://youtube.com/playlist?list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t&si=UEx182w7ZJc_lHu1](https://youtube.com/playlist?list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t&si=UEx182w7ZJc_lHu1)


### Data Acquisition
- Data was uploaded locally from a csv file.
- Dataset contained colu
### Data Cleaning
- Removed entries with null values and incorrectly entered values
- Made new columns to find out if different skills were included in the job description
- Created new column for simplified job title
- Parsed out the ratings for different companies
- Created a column to find out which state the job posting was in
- Created column for description length


### EDA
Explored the data to find key patterns and insights. Crucial points discussed below. Detailed look inside the jupyter notebook.
![](https://github.com/WasiShaikh977/Data-Science-Salary-model/blob/main/wordcloud.png)


### Building the Model
- After cleaning the data, transformed the categorical columns into dummy variables, standardized the continuous variables and then split it into a training and a testing dataset.
- Trained on 3 different regression models - Linear Regression, Lasso and Random Forest.
- Used GridSearchCV to optimize our best model (Random Forest) even futher.
- 

### Model Performance
 - RandomForestRegressor had the best performance on the training dataset and it seems to have generalized well. Giving us an even better performance on the testing dataset with mean absolute error of 10.06. A very respectable number when we compare it to the estimated salary ranges in our original dataset.
- Lasso performed okay, similar to the training results. Its MAE on the testing data was 17.11.
- As for Linear Regression, it failed as a model. Giving us unreasonably high training and testing MAE. We can not consider it at all.


### Conclusion
##### Key Insights from EDA
- Python is as key programming software for a person looking to work in the field of Data Science or any other data related roles.
- People with Python and Machine Learning skills stand a good chance of earning an above average to a every good salary.
- California, DC and New York came out as the best locations overall taking into account the number of openings and the estimated salary.
- Low to low-mid tier companies seem to be hiring a high number of people in data related jobs whereas the public companies are the ones giving out the highest salaries

##### Modelling Performance
- Linear Regression: Extremely poor performance
- Lasso: 15.68 MAE (Decent)
- Random Forest: 10.06 MAE (Good)
