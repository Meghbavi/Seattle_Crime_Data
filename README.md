SEATTLE CRIME DATA PREDICTION

Introduction:

Criminality is one of the most tough social problems, and it has gotten worse as the population has grown. The elements that contribute to an increase in criminal activity must be understood by security authorities. Because they are working on a range of issues, officials may not be able to predict future crimes. Despite their greatest efforts, officials and police officers may not be able to totally reduce crime rates. Crime prediction is one of the main activities of criminology, which entails predicting crime incidence, recognizing crime trends, and connecting them to other horrifying episodes and criminal organizations.Law enforcement agencies' biggest challenges are criminal identification and crime prediction. It is nearly impossible for security authorities to manually investigate and unravel concealed criminal trends due to the massive volume of data, complexity, and rising crime rate. To solve this challenge, new technology is required that can accurately forecast crime and identify crime patterns.

Project Objective and Problem Statement:

 It is to predict at what time of the day the crimes are most likely to happen. So that the law enforcement agencies can save or stop the crime which will have in future. They can stop the future crimes.


# Seattle_Crime_Data

Seattle Crime Data Analysis. In this Project I used Seattle crime data to do exploratory analysis and provide statistical answers to the issues. 
Dataset contains the following columns: Report Number: Unique report number for the record. 
Offense Id : When a single report contains several violations, a unique identification is used to indicate this.
Offense Start DateTime: Offense start time and date.
Offense End DateTime: End date and time of offense.
Report DateTime: Date and time the offenses was reported.
Group A B: offense group
Crime Against Category: offense crime of each category.
Offense Parent Group: Parent group of offense.
Offense: Crime or offense reported.
Offense Code: Code of offense
Precinct: Where the offenses occurred is indicated with a police precinct boundary.
Sector: Where the offenses happened, a police sector boundary was designated.
Beat: Designated police sector boundary where offense(s) occurred.
MCPP:Where the offenses happened, there is a designated Micro-Community Policing Plans (MCPP) boundary.
100 Block Address:The location of the offenses has been obfuscated to the hundred block.
Longitude: The spatial coordinates of the offenses were blurred to the hundred block.
Latitude: The spatial coordinates of the offenses have become hazy up to the hundred block.

DATASET SOURCE:
https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5/data

Project Implementation:

Exploratory Data Analysis:

1)I have changed the name of the columns for easy use.
2)Checking missing and null values and replacing the Nan values if neccessary with approriate value.
3)Dropping the uneccessary columns and checked for duplicate values.
4)Changing the Datatypes to correct type.
5)Performed visualizations to check the null values, to understand which category has the highest and least crimes. Also, based on the two Groups A and B which group had the highest crime rate in Group A and Group B
6) Also, when were the most crimes happened during day time or midnight?
7) Checking which areas use the mccp plans more and less.

Modelling:

Logistic Regression:

For grid search, C values of [0.001,0.1,1] were employed as hyperparameters.
When hyperparameter C is 0.001, the model appears to be the best fit.
Because the target variable is significantly skewed, accuracy of 84% .
The AUC of the ROC curve is 90%.

Random Forest:

Modeling hyperparameters: utilized max_depth values of [15,17].
The model appears to work best with a value of 10 for n neighbors.
The model has a 99 percent accuracy rating, which is greater than the logistic regression model.
The area under the curve has been raised to 100%, which is lower than logistic models.

Conclusion:

I couldnt give proper conclusion because my randomforest AUC and validation are nearly 100, that means there might be overfitting concern in the dataset which i have used. But Overall, I would recommend to use RandomForest model as it has the highest accuracy and AUC score. Also, RandomForest is the better approach if there is lots of imbalances in the data. And most of my data is categorical type, So, Randomforest performs much better than logistic regression for categorical data.

