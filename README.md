# MechaCar_Statistical_Analysis

## Linear Progression to Predict MPG
As you can see in the [Linear Regression](MechaCar_linear_regression.png) calculation, the vehicle length and ground clearance are unlikely to provide random amounts of variance to the model. The slopes of th vehicle length and ground clearance shows positive corelation between the two categories and mpg. The p-value is 5.35 x 10-1, which is much smaller than the assumed significance level of 0.05%. Therefore, we can state that there is sufficient evidence to reject the null hypothesis, which means that the slope of our linear model is not zero. Although the two variables are positively correlated, the high significance value of the Intercept is evidence of overfitting. This means that them model cannot be used to predict a future dataset correctly.

## Summary Statistics on Suspension Coils
Looking at the [Total Summary Table](total_summary.png), at first glance it looks like the coils in the dataset are within the required variance that MechaCar dictates. The variance is 62.29. In order to get more detail on the data, I used the group_by() function to group the coils by thier respective manufacturing lot. When you look at the variance of the [Lot Summary](lot_summary.png), you can see that the suspension coils in lot3 have a variance of 170.27, and therefore do not meet the requirements. 

## T-Tests on Suspension Coils
To determine if the suspension coil's PSI results are statistically different from the mean population, I conducted four one-sample t-tests. The first t-test I conducted looked at the PSI across all manufacturing lots to see if they were statistically different from the population mean of 1,500. Looking at the [Total T-Test](total_t_test.png), you can see that the p-value is 1, which means that the two means are statistically similar. Next I looked at [Lot1](subset1_t_test.png), which had a p-value of 1.56 x 10-11, [Lot2](subset2_t_test.png), which had a p-value of .00059, and [Lot3](subset3_t_test.png), which had a p-value of 0.15. Based on these values, for Lot1 and Lot2, we can state that there is sufficient evidenct to reject the null hypothesis.

## Study Design: MechaCar vs Competition
Another study that could be conducted to determine whether the fuel efficency of a MechaCar has
an impact on the cost of the car. When I bought my first car, those were the two things most important to me in making my decision. For this analysis, my null hypthesis is that miles per gallon increases the cost of the car. I would run a t-test to determine the mpg are statistically related. The data that I would need would be the cost of each of the MechaCar's.  
