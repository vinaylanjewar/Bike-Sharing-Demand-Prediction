# Bike-Sharing-Demand-Prediction

### **Problem statement** : 
It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. This project tackles the problem of predicting the number of bikes which will be rented at any given hour in a given city. The main objective is to build various regression models and analyze their performance with respect to each other so as to get the best performing model, which could help in predicting the number of bikes required at each hour for the stable supply of rental bikes.

### **Data set Description**:

* Date : year-month-day
* Rented Bike count - Count of bikes rented at each hour
* Hour - Hour of the day
* Temperature-Temperature in Celsius
* Humidity - %
* Windspeed - m/s
* Visibility - 10m
* Dew point temperature - Celsius
* Solar radiation - MJ/m2
* Rainfall - mm
* Snowfall - cm
* Seasons - Winter, Spring, Summer, Autumn
* Holiday - Holiday/No holiday
* Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

### **Factors Affecting**:

1.	Seasons : Bike rental is high during the summer and least during the Spring season.

2.	Temperature : As the temperature increases the bike count is gradually increases .

3.	Hours : We observed that there is a peak in the bike rentals counts at around 8am morning and at around 5pm evening.

4.	Weather :  When the weather is clear or sunny the bike rental is high where as in the heavy rain and snowfall the bike rental is very low.

5.	Working Day : Bike rental counts on working and non-working days and we observed that the outliers are present in working day.

6.	Holiday : Bike rental counts on holidays and non-holidays. Holidays correspond to non-working days. Also outliers are present in non holidays.

### **Steps Involved**:

1.	Exploratory Data Analysis : 
After loading and reading the dataset in notebook, we performed EDA. Comparing target variable which is bike rentals counts with other independent variables.
This process helped us figuring out various aspects and relationships among the target and the independent variables and also we observed the distribution of variables.
It gave us a better idea that how feature behaves with the target variable.

2.	Preprocessing data  :
Dataset contains a no null values also no duplicate values are found to disturb the accuracy .
Changing column names for easy handling.
Dropping the unwanted columns from the dataset.

3.	Features selection :
With the help of exploratory data analysis we analyzed the categorical as well as numerical features in the dataset.

4.	One hot encoding :
In this dataset some categorical variables like seasons, holiday and function day, we change it with numerical database.

5.	Correlation Analysis :
We plot the heatmap to find  the correlation between both dependent variable and independent variables.

6.	Train test Split :
In train test split we take ‘x’ as dependent variables and ‘y’ take as independent variable then train the model.

### **Correlation Analysis**:

![corre](https://user-images.githubusercontent.com/96326032/172069435-55576b6e-914c-4b58-94ad-9cf98643fe4b.png)

### **Conclusion** :

1.	Bike rental count is mostly correlated with the time of the day as it is peak at 10 am morning and 8 pm at evening. 
2.	We observed that bike rental count is high during working days than non working day.
3.	We see that people generally prefer to bike at moderate to high temperatures. We observed highest rental counts between 32 to 36 degrees Celsius.
4.	It is observed that highest number bike rentals counts in Autumn/fall Summer Seasons and the lowest in Spring season.
5.	We observed that the highest number of bike rentals on a clear day and the lowest on a snowy or rainy day.
6.	We observed that with increasing humidity, the number of bike rental counts decreases.
7.	Hour of the day holds most importance among all the features for prediction of dataset.
