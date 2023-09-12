# Prediction-of-Product-Sales
- Cheyenne Cantwell
#
###Business Problem:
- The goal is to help the retailer understand the properties of products and outlets that play crucial roles in increasing sales. To do this I need to analyze the data and predict future sales of products.
#
###Data:
- This is the data used: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view?usp=sharing
- This data comes from this source: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/
# 
##Methods:
- After cleaning up the data I explored the data using different vizualizations, a couple seen below:
#
![image](https://github.com/SpreeC/Prediction-of-Product-Sales/assets/137640455/dd29c4fb-9ddf-4ec0-ae6e-198d702ef70c)
##### Through this visualization we can see that Item_MRP and Item_Outlet_Sales have a positive correlation; and Item_Visibility and Item_Outlet_Sales have a negative correlation
# 
![image](https://github.com/SpreeC/Prediction-of-Product-Sales/assets/137640455/e3c659e5-d227-4ee2-9327-31794d83c266)
##### This visualization gives us more detail into the positive correlation of Item_MRP and Item_Outlet_Sales
#
- After exploring my data I then had to pre-process it for machine learning and in doing so I found that there were missing values for Item_Weight and Outlet_Size. I decided to impute Outlet_Size with NA because it was missing 28.28% of values. I then imputed Item_Weight with median as it was missing 17.17% of values and this would best represent the Item_Weight because it did not have any outliers to skew the data.
- After pre-processing I then ran two different models, Linear Regression and Random Forest.
#
##Model:
- I recommend the Random Forest Model because the training data did better when compared with the linear regression and the test data did better than the linear regression after tuning the model. Looking at the R-squared figure we can see that the Random Forest Model is the best for the job because both the testing and the training data did better than the linear regression model. For the r-squared we can see that about 60% of the variance is explained. Looking at the RMSE for the test data, we have an error rate of $1,050.19. I chose this metric because it best represents the error rate in the model by punishing the larger errors and it is easy to interpret as it is in the original units of the target (Product Sales is in dollars).
#
##Recommendations:
- I recommend trying to balance the model and try to tune it after balancing it. It is possible that using a different model could do better with the data as well.
#
###For Further Information:
- For any additional questions, please contact cheyenne.cantwell@gmail.com
