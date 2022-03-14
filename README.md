# COMP4447-Final-Project
Repository for final group project for Data Science Tools 1

### GROUP MEMBERS
- Abigail Ward
- Arun Joseph
- Navan Powers

### Dataset 
This dataset came from an online survey at askamanager.org (https://www.askamanager.org/2021/04/how-much-money-do-you-make-4.html) . The goal of this survey was to take the mystery out of salaries and allow people to see how much others were actually making. There are 17 variables consisting of: 
Timestamp	
How old are you?	
Industry	
Job title	
Additional context on job title	
Annual salary	
Other monetary comp	
Currency	
Currency - other	
Additional context on income	
Country	
State	
City	
Overall years of professional experience	
Years of experience in field	
Highest level of education completed
Gender	
Race		

This dataset was downloaded from https://docs.google.com/spreadsheets/d/1IPS5dBSGtwYVbjsfbaMCYIWnOuRmJcbequohNxCyGVw/edit?resourcekey#gid=1625408792. At the time the dataset was downloaded for use in this analysis there were 27680 responses. 				

### Research Question
How accurately can salary be predicted based on the features in this dataset? What are the best predictors of salary? 

### Literature review
This work is different than other studies, because our salary includes all types of income including non-conventional earnings. Additionally, there is a strong bias in this dataset toward women and US citizens. 

### Quality of cleaning 
Many of the fields in this dataset were free-text that needed to be filtered into specific categories. Title and Industry required NLP to breakdown the text into its core topics. Salary needed to account for people who entered improbable values and conversioin into a common currrency. Location such as city and state were used to fill in missing values in country. 
It was attemted to fill in all missing values using information from other fields. If the row contained a missing value after cleaning, that row was removed.  

### Visualization
To understand the dataset, a pandas profiling report was made, as well as a correlation heat map. After the Random Forest Regression was fit, feature importance and residuals were plotted. The model has an r-squared value of 0.364 implying the initial model does not fit the data well. 
