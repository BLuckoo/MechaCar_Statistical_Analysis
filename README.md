## MechaCar_Statistical_Analysis

### **Overview of Project:**

**To help AutosRUs' manufacturing team with the newest prototype, MechaCar, the following statistical analysis has been performed on data collected by the production team:**
- Multiple linear regression analysis to identify which variables in the dataset predict the mpg of the MechaCar prototypes;
- Collection of summary statistics on the pounds per inch of the suspension coils from the manufacturing lots;
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population;
- Design a statistical study to compare performance of the MechaCar against vehicles from other manufacturers.

### **Results of Analyses**

**1.  Linear Regression to predict MPG**

To determine whether the fuel consumption, measured in miles per gallon (mpg), a multiple linear regression was applied to the data collected by the production team.

The following image shows the model that was used with the variables provided, i.e.:
  - vehicle length
  - vehicle weight
  - spoiler angle
  - ground clearance
  - all wheel drive (AWD) or not

![image](https://user-images.githubusercontent.com/82583576/127779743-8f62e66d-5be6-4527-9ed5-d9841feb52a4.png)

***The results of the model shows the following:***
1. Most significant variables in the dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. 
   As indicated by the green arrows in the image above, a linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10<sup>-12</sup>      and 5.21x10<sup>-8</sup>, respectively. 
   The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.
   
2. The slope of the linear model can not be considered to be zero, as the p-value of 5.35x10<sup>-11</sup>, indicated by the blue arrow above, is lower than even an extreme        level of significance, and thus the null hypothesis must be rejected. This means that the relationship between the variables and the miles per gallon is subject to more than     random chance.

3. This model does predict the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149, highlighted in the red box, indicates that the        model is 71.5% accurate.




