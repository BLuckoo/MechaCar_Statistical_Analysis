## MechaCar_Statistical_Analysis

### **Overview of Project:**

**To help AutosRUs' manufacturing team with the newest prototype, MechaCar, the following statistical analysis has been performed on data collected by the production team:**
- Multiple linear regression analysis to identify which variables in the dataset can be used to predict the miles per gallon (MPG) of the MechaCar prototypes;
- Collection of summary statistics on the pounds per inch of the suspension coils from the manufacturing lots;
- Run T-Tests to determine if the manufacturing lots are statistically different from the mean population;
- Design a statistical study to compare performance of the MechaCar against vehicles from other manufacturers.

### **Results of Analyses**

### **1.  Linear Regression to predict MPG**

To determine whether the fuel consumption, MPG, can be predicted using certain variables, a multiple linear regression was applied to the data collected by the production team.

The following image illustrates the model that was used with the variables provided, i.e.:
  - vehicle length
  - vehicle weight
  - spoiler angle
  - ground clearance
  - all wheel drive (AWD) or not

<p align="center">
<img width="750" src="https://user-images.githubusercontent.com/82583576/127779743-8f62e66d-5be6-4527-9ed5-d9841feb52a4.png">
</p>


  ***The results of the model shows the following:***

A. Vehicle Length and Ground Clearance were the most significant variables in the dataset with non-random effect on the MechaCar MPG. 
   As indicated by the green arrows in the image above, a linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10<sup>-12</sup>      and 5.21x10<sup>-8</sup>, respectively. 
   The intercept was also statistically significant, indicating that there are likely other factors, not included in the dataset, that have a strong impact on the MPG.
   
B. The slope of the linear model cannot be considered to be zero, as the p-value of 5.35x10<sup>-11</sup>, indicated by the blue arrow above, is lower than even an extreme          level of significance, and thus the null hypothesis must be rejected. This means that the relationship between the variables and the miles per gallon is subject to more than    random chance.

C. This model does predict the MPG of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149, highlighted in the red box, indicates that the        model is 71.5% accurate.


### **2.  Summary Statistics on suspension Coils**

***Total Summary Statistics for Suspension Coils PSI***

<p align="center">
<img width="750" src="https://user-images.githubusercontent.com/82583576/127781893-f40c5c87-057c-4307-a604-f8d69a45721b.png">
</p>

- As per the table above, for the suspension coil's PSI continuous variable, the mean and median are nearly same. This is an indication that the dataset has a normal (symmetric) distribution and it does not have any skewness.
- A high standard deviation (7.89) indicates that the data points are spread out over a large range of values.
- As per the design specifications for the MechaCar suspension coils, the variance must not exceed 100 PSI. As per the above statistics, the variance is about 62 PSI, well below the specified value. Hence the current manufacturing data meets this design specification.


***Summary Statistics for Suspension Coils PSI by Lot***
<p align="center">
<img width="750" src="https://user-images.githubusercontent.com/82583576/127781911-916ce20a-b55c-43fe-a8cf-eaf6725bde9e.png">
</p>

- The mean and median for the three lots are all very close, indicating that for each of the lots the dataset does not show any skewness.
- The standard deviations for Lot 1 and Lot 2 are relatively small - an indication that the data points for these two lots are close to each other.
- The standard deviation for Lot 3 is relatively higher than the standard deviation for Lot 1 and Lot 2, meaning that the data points for lot 3 are further spread out than Lot 1 and Lot 2.
- The variances for Lot 1 and Lot 2 are relatively low and within the acceptable level set by the design specfication.
- However, the variance for Lot 3 is at 170.28 and therefore is well over the acceptable threshold of 100 psi. This is an indication of possible flaws in the production of those suspension coils.


### **3. T-Tests on suspension Coils**

***A. Suspension Coils Cummulative T-Test***

In this case, the one-sample t-test has been used to assert if there is a statistical difference between the means of a sample dataset (suspension coil's pound-per-inch) and hypothesized, potential population dataset. The mean of the hypothesized, potential population dataset is given as 1,500 pounds per inch.

<p align="center">
<img width="750" src="https://user-images.githubusercontent.com/82583576/127782351-2a14ad56-6fb3-4052-8466-910e54f839aa.png">
</p>

- A review of the results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) to reject the null hypothesis. The two means are statistically similar.


***B. Suspension Coils T-Test for Lot 1***

<p align="center">
<img width="750" src="https://user-images.githubusercontent.com/82583576/127783071-a17d067f-575d-438a-9e3f-5daa5150d5c9.png">
</p>

- A review of the results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) to reject the null hypothesis. 

***C. Suspension Coils T-Test for Lot 2***

<p align="center">
<img width="750" src="https://user-images.githubusercontent.com/82583576/127783084-548a02e4-2142-457e-a951-d89a9471a716.png">
</p>

- A review of the results of the T-test for the suspension coils for Lot 2 indicates that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) to reject the null hypothesis.


***D. Suspension Coils T-Test for Lot 3***

<p align="center">
<img width="750" src="https://user-images.githubusercontent.com/82583576/127783099-3208c15a-d15d-409a-a996-d7606b3b247c.png">
</p>

- 	A review of the results of the T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough (0.0417) to reject the null hypothesis. 

- This lot may be need to be discarded, or at least more closely evaluated.


### **4. Study Design: MechaCar vs Competition**

Consumers take many factors into consideration when evaluating a car to purchase. 
Some of the metrics that are of interest to a consumer would include cost of ownership, fuel efficiency, carrying capacity and colour options. 
By getting a good handle on these metrics and making sure that MechaCar satisfies the findings, AutosR'Us can outperform the competition.

These metrics and the statistical tests that could be performed are listed in the table below:

<p align="center">
<img width="953" src="https://user-images.githubusercontent.com/82583576/127786116-387d1745-1cbb-49a2-86de-f2027e22df38.png">
</p>

#### The Data Analysis team looks forward to continue working with the Production teams on the analysis of additional data. This will help to improve the MechaCar prototypes to a successful commercialisation!

