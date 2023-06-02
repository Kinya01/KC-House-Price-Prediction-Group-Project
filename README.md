# **Kingston County House Data Analysis**
# Objective 
In this project, we examined the different factors that impact the pricing of houses in King's County. According to our best predicting multiple regression model, squarefoot living and the grade were the best predictors of housing prices in Kingston county
# **Python Library Tools**
- Pandas
- Numpy
- Seaborn
- Matplotlib
- Scikit Learn
- Statsmodels
# **Data**
The dataset utilized in this project was obtained in CSV format from Kaggle, consisting of 20,000 data points. The dataset includes the following features: id, date, price, bedrooms, bathrooms, sqft_living, sqft_loft, floors, waterfront, view, condition, grade, sqft_above, sqft_basement, yr_built, yr_renovated, zipcode, latitude, and longitude.
![image](https://github.com/Kinya01/Kinya01/assets/128283613/8d202afe-5e2e-42c9-868f-a57399bc9f69)
# **Data Correlation**
We took a better look at the data correlation
![image](https://github.com/Kinya01/Kinya01/assets/128283613/6231cb60-8b8c-49a5-8cd4-b9863756e858)
These were the top correlation Features
![image](https://github.com/Kinya01/Kinya01/assets/128283613/9feb3be9-59e4-41d5-b3e0-f87fa626bfda)
# **Modelling**
We used a simple linear regression model to depict the relationship between sqft_living(highest correlation feature) and price
![image](https://github.com/Kinya01/Kinya01/assets/128283613/1742f75a-e0be-49a7-a733-ea2d84ed3efa)
For the multiple regression model, we used two models to conduct a multiple linear regression analysis between the price, waterfront, sqrft_living and bathrooms and we picked the second model since it had higher accuracy of 0.899
# **Results**
R-squared (uncentered): The R-squared value of 0.899 indicates that the model explains approximately 89.9% of the variance in the dependent variable (price). This suggests that the independent variables included in the model (bathrooms, sqft_living, waterfront) collectively have a strong association with the price.

Adjusted R-squared (uncentered): The adjusted R-squared value is also 0.899, which means that the inclusion of the three independent variables in the model is not significantly impacting the overall goodness of fit. The adjusted R-squared value is useful for comparing models with different numbers of predictors.

F-statistic: The F-statistic has a very large value of 6.378e+04, and the associated probability (Prob (F-statistic)) is 0.00. This indicates that the overall model is statistically significant, suggesting that at least one of the independent variables has a significant impact on the price.

Coefficients: The coefficients for the independent variables indicate the magnitude and direction of their relationship with the dependent variable (price).

Bathrooms: The coefficient for the "bathrooms" variable is 4.4689, indicating a positive relationship with the price. A one-unit increase in the number of bathrooms is associated with an increase in the price by approximately 4.4689 units.

Sqft_living: The coefficient for the "sqft_living" variable is 0.0011, indicating a positive relationship with the price. A one-unit increase in the square footage of living area is associated with an increase in the price by approximately 0.0011 units.

Waterfront: The coefficient for the "waterfront" variable is -1.3921, indicating a negative relationship with the price. A property with a waterfront location is associated with a decrease in the price by approximately 1.3921 units.

All three variables have p-values close to zero, indicating that they are highly statistically significant in relation to the price.
# **Recommendations**
Stakeholders should consider:
- Including a larger living area for their house rennovations since it fetches a higher price
- Including more bathrooms in their house rennovations since price increases with increase in the number of bathrooms depending on our final model
- Excluding a waterfront from their houses during rennovations or buying houses without a waterfront. This is becauase according to our final multiple regression model, the waterfront is negatively correlated with price.

