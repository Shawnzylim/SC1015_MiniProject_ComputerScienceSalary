# SC1015_MiniProject_ComputerScienceSalary
## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on predicting salary given different factors in the Computer Science industry.
## Dataset
We combined two datasets
[Job_skills_qualifications.xlsx](https://github.com/Shawnzylim/SC1015_MiniProject_ComputerScienceSalary/files/8546509/Job_skills_qualifications.xlsx)
and
[title_location_company_salary.xlsx](https://github.com/Shawnzylim/SC1015_MiniProject_ComputerScienceSalary/files/8546510/title_location_company_salary.xlsx).
## Project Aim and Motivation
This project aims to use certain factors in a persons job in the computer science industry to determine the salary that they will have.
## Contributors
- @Shawnzylim - Presentation, Code
- @chenyiming - Slides
## Project Overview
### 1. Problem Definition
- As computer science students what fields and jobs are best paid in our future careers?
- Are there important skillsets and talents we need to get in order to command higher slaries?
- Which model can we use to predict salaries?
### 2. Data Extraction & Exploratory Data Analysis
- Concatenated the two datasets together
- Removing duplicate columns
- Deleting variables that are unhelpful
- Removed *NULL* value rows
- Removed outliers in salaries
- Using boxplot and barplot to visualise the data
- Statistical distribution of Salary
- Checked the importance of having python skillset on Salary
### 3. Feature Engineering
- Categorical data had to be converted to numerical for the sake of machine learning
- Ensure that the different skillsets have been one-hot encoded into '1' meaning they are proficient and '0' being inept
- Noticed that the different unique jobs, cities and companies were to large for one-hot encoding
- They had to be label encoded instead
### 4. Model Building
-  Built and tested Random Forest Regression machine learing algorithms
-  Tested accuracy of the model using Mean absolute error and mean percentage error
-  Random Forest had a very high accuracy of 90.27%
### 5. Conclusion
- Feature engineering to enable us to use regression
- We discovered that in terms of importance of the factors in predicting the salary, the most important factor was which company the person was working at and coming in second was surprisingly whether the person had a doctorate in philosophy
### 6. New Insights Learned
- Learning how to filter the data using label encoding and outliers removal
- Random Forest Regression
- By using only the two most important variables company and doctor in philosophy, the accuracy of the model was still very high at 87.62%
## References
1. https://towardsdatascience.com/random-forest-in-python-24d0893d51c0
2. https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
3. https://pbpython.com/categorical-encoding.html
4. https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html
