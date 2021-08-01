## MechaCar_Statistical_Analysis

### **Overview of Project:**

**To help AutosRUs' manufacturing team with the newest prototype, MechaCar, the following statistical analysis has been performed on data collected by the production team:**
- Multiple linear regression analysis to identify which variables in the dataset predict the miles per gallon (MPG) of the MechaCar prototypes;
- Collection of summary statistics on the pounds per inch of the suspension coils from the manufacturing lots;
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population;
- Design a statistical study to compare performance of the MechaCar against vehicles from other manufacturers.

### **Results of Analyses**

**1.  Linear Regression to predict MPG**

To determine whether the fuel consumption, MPG, can be predicted using certain variables, a multiple linear regression was applied to the data collected by the production team.

The following image shows the model that was used with the variables provided, i.e.:
  - vehicle length
  - vehicle weight
  - spoiler angle
  - ground clearance
  - all wheel drive (AWD) or not

![image](https://user-images.githubusercontent.com/82583576/127779743-8f62e66d-5be6-4527-9ed5-d9841feb52a4.png)

***The results of the model shows the following:***
A. Most significant variables in the dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. 
   As indicated by the green arrows in the image above, a linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10<sup>-12</sup>      and 5.21x10<sup>-8</sup>, respectively. 
   The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.
   
B. The slope of the linear model cannot be considered to be zero, as the p-value of 5.35x10<sup>-11</sup>, indicated by the blue arrow above, is lower than even an extreme          level of significance, and thus the null hypothesis must be rejected. This means that the relationship between the variables and the miles per gallon is subject to more than    random chance.

C. This model does predict the MPG of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149, highlighted in the red box, indicates that the        model is 71.5% accurate.


**2.  Summary Statistics on suspension Coils**

*Total Summary Statistics for Suspension Coils PSI*

![image](https://user-images.githubusercontent.com/82583576/127781893-f40c5c87-057c-4307-a604-f8d69a45721b.png)

The Total Summary data above, shows that the overall PSI variance in under 100 psi and meets specifications.

*Summary Statistics for Suspension Coils PSI by Lot*

![image](https://user-images.githubusercontent.com/82583576/127781911-916ce20a-b55c-43fe-a8cf-eaf6725bde9e.png)


However, based on the Lot Summary statistics, the variance for Lot 3 is well over the acceptable threshold at 170.28.





