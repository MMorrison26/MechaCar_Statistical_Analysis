# MechaCar Statistical Analysis

## *Linear Regression to Predict MPG*
1) The variables/coefficients that have a non-random amount of variance to the mpg values in the dataset include: the ground_clearance (-0.463776) and the AWD (0.406308). The vehicle_weight (-0.000170) and spoiler_angle (-0.009066) are too close to zero to have any significant (non-random) affect on the mpg.
2) The p-value here is 6.712e-11, which is much smaller the the assumed significance level of 0.05%. This means we can reject the null hypothesis, which means that the stlope of our linear model is not zero.
3) Given that the r-squared value for this linear model is 0.7119, this model predicts MechaCar prototypes pretty effectively, meaning that roughly 71% of the variability of our dependent variable is explained using this linear model. <br/>

![image](https://user-images.githubusercontent.com/87578449/143689841-082a0970-27b8-4124-bfad-3281898fcda6.png)


## *Summary Statistics on Suspension Coils*
If you take a look at the overall summary and lot-by-lot summary tables below, you can see that yes, the variance overall does not exceed 100 pounds per square inch (with a variance of 62.29), but it does not work for each lot individually. Lots 1 and 2 hit the variance qualificiation (with variance of 0.98 and 7.47 respectively), but Lot 3 has a variance of 170.29, which greatly exceeds that 100 pounds per square inch. <br/>

![image](https://user-images.githubusercontent.com/87578449/143689637-452d5ef1-200f-48ad-b1e2-8134a0495e3c.png) <br/>
![image](https://user-images.githubusercontent.com/87578449/143689642-dfc2da64-f3b8-4937-9944-159fa5883539.png) <br/>
