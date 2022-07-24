# MechaCar_Statistical_Analysis
 
## Linear Regression to Predict MPG

**Statistical Summary:** 
![d1](https://github.com/vvinci21/MechaCar_Statistical_Analysis/blob/aebe0501b5f21fd9fc1a091972c6a8b6427439dc/deliv_1%20Small.png)

From the above output we can see that:

1. The **vehicle length**, and **vehicle ground clearance** are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely,
the **vehicle weight**, **spoiler angle**, and **All Wheel Drive** (AWD) have p-Values that indicate a random amount of variance with the dataset.  

2. The p-Value for this model, ```p-Value: 5.35e-11```, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to **reject our null hypothesis**, which further indcates that the slope of this linear model is **not zero**.


3.  This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. Relatively speaking, his multiple regression model **does predict mpg of MechaCar prototypes effectively**. 

  
## Summary Statistics on Suspension Coils

![total_sum](https://github.com/vvinci21/MechaCar_Statistical_Analysis/blob/aebe0501b5f21fd9fc1a091972c6a8b6427439dc/total_summary%20Small.png)

![d2](https://github.com/vvinci21/MechaCar_Statistical_Analysis/blob/aebe0501b5f21fd9fc1a091972c6a8b6427439dc/lot_summary%20Small.png)

With the understanding that the design specifications for the MechaCar suspension coils mandate that <mark style="background-color: Yellow">**the variance of the suspension coils cannot exceed 100 pounds per square inch (PSI)**</mark> . 


When looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement.  

Similarly, but significantly more consistent, Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47 respectively.  However, it is Lot 3 that is showing much larger variance in performance and consistency, with a variance of 170.29.  It is Lot 3 that is disproportionately causing the variance at the full lot level.  

This very simple boxplot illustrates the differences between the lots:


## t-Tests on Suspension Coils

There is a summary of the t-test results across **all manufacturing lots**

From here we can see the **true mean of the sample is 1498.78**, which we also saw in the summary statistics above.  With a **p-Value of 0.06**, which is higher than the common significance level of 0.05, there is **NOT enough evidence to support rejecting the null hypothesis**.  


1. Lot 1 sample actually has the **true sample mean of 1500**, With a **p-Value of 1**, we cannot reject the null hypothesis.

2. Lot 2 has the same outcome with a **sample mean of 1500.02**, a **p-Value of 0.61**; the null hypothesis cannot be rejected.

3. Lot 3, **the sample mean is 1496.14** and the **p-Value is 0.04**, which is lower than the common significance level of 0.05.  All indicating to **reject the null hypothesis** that this sample mean and the presumed population mean are not statistically different.


Something was different in in Lot 3's manufacturing cycle. The process needs quality and standard checks and the suspension coils from this lot need to be inspected to remove those not meeting quality criteria.


## Study Design: MechaCar vs Competition

#### Metrics
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

*  Current Price (Selling): **Dependent Variable**
*  Average Annual Cost of ownership (Maintenance): **Independent Variable**
*  MPG (Gasoline Efficiency): **Independent Variable**


#### Hypothesis: Null and Alternative
After determining which factors are key for the MechaCar's genre:

 * Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
 * Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.
 
#### Statistical Tests
A **multiple linear regression** would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price.
