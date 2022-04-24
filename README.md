# Welcome to our SC1015 Data Science Mini Project!

## About
This is a data science project done for our SC1015 Module (Introduction to Data Science and Artificial Intelligence) which focuses on two data sets. A .csv file containing the listing information from Airbnb's website and feature engineering the GeoData of tourist attractions from Data.gov.sg .

Please view our code in the notebook.ipynb.

### Contributors
- Moe Thu - Data Preparation & Cleaning, Exploratory Data Analysis, Linear Regression, XGBoost, Random Forest Regression, Presenter
- Woon Kit - Data Preparation & Cleaning, Exploratory Data Analysis, ElasticNet Regression, Presentation Slides, Presenter
- Zhong Han - Data Preparation & Cleaning, Exploratory Data Analysis, Support Vector Machines, Presentation Slides, Presenter

### Problem Definition and Motivation
Airbnb is a service that lets homeowners rent out their property for travellers to stay, in Singapore this focuses on tourists/foreigners. In addition, we tested whether the "distance from tourist attraction" variable would be helpful in predicting price. 

*Our Hypothesis:*
 1. Most of the people on Airbnb are travellers
 2. They would want to have a location near tourist attractions as less travel time would be needed
 3. Thus increasing the demand and raising the price of those Airbnbs.
 4. We realised this would be important as it could help hosts know the value of their house better
 
### Models Used
- Linear Regression
- Random Forest Regression
- XGBoost
- Support Vector Machines
- ElasticNet Regression

### Conclusion
- Distance between airbnb and tourist attraction correlates weakly, perhaps this is due to Singapore being small such that distance does not matter as much.
- It solves our original problem, as we were able to determine that distance from tourist attractions is not the best indicator.
- However, it still performed quite well for the random forest regression model, so it would be useful in models using random forest regression.
- Overall our best model for predicting AirBnb prices to help hosts would be random forest regression, and the best variables would be beds, bedroom, accommodates. 
- We believe that those three variables, correlate the amount of space that is rented as having more bedrooms, beds and people would naturally mean more space is required to rent, thus amount of space rented is missing.

### Learning Outcome
*What we have learned is that:*
- We initially used label encoding to convert categorical to numerical, but we cannot just use any encoding function on data, for our case, since our data was not ordinal, we had to use one-hot encoding instead.
- Important to know what you want to do ahead of time, as we had a variable that counts the nearest amount of tourist attractions within 5km but it showed little correlation to price, so we scrapped that.

### References
1. https://androidkt.com/detect-and-remove-outliers-from-pandas-dataframe/
2. https://www.analyticsvidhya.com/blog/2020/03/one-hot-encoding-vs-label-encoding-using-scikit-learn/
3. https://stackoverflow.com/questions/41325227/how-to-do-linear-regression-using-python-and-scikit-learn-using-one-hot-encoding
4. https://www.analyticsvidhya.com/blog/2018/09/an-end-to-end-guide-to-understand-the-math-behind-xgboost/
5. https://www.datacamp.com/community/tutorials/xgboost-in-python
6. https://towardsdatascience.com/random-forest-in-python-24d0893d51c0
6. https://stackabuse.com/implementing-svm-and-kernel-svm-with-pythons-scikit-learn/
7. https://www.datatechnotes.com/2019/08/elasticnet-regression-example-in-python.html