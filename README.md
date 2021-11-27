# MechaCar Statistical Analysis

## *Linear Regression to Predict MPG*
1) The variables/coefficients that have a non-random amount of variance to the mpg values in the dataset include: the ground_clearance (-0.463776) and the AWD (0.406308). The vehicle_weight (-0.000170) and spoiler_angle (-0.009066) are too close to zero to have any significant (non-random) affect on the mpg.
2) The p-value here is 6.712e-11, which is much smaller the the assumed significance level of 0.05. This means we can reject the null hypothesis, which means that the stlope of our linear model is not zero.
3) Given that the r-squared value for this linear model is 0.7119, this model predicts MechaCar prototypes pretty effectively, meaning that roughly 71% of the variability of our dependent variable is explained using this linear model. <br/>

![image](https://user-images.githubusercontent.com/87578449/143689841-082a0970-27b8-4124-bfad-3281898fcda6.png)


## *Summary Statistics on Suspension Coils*
If you take a look at the overall summary and lot-by-lot summary tables below, you can see that yes, the variance overall does not exceed 100 pounds per square inch (with a variance of 62.29), but it does not work for each lot individually. Lots 1 and 2 hit the variance qualificiation (with variance of 0.98 and 7.47 respectively), but Lot 3 has a variance of 170.29, which greatly exceeds that 100 pounds per square inch. <br/>

![image](https://user-images.githubusercontent.com/87578449/143689637-452d5ef1-200f-48ad-b1e2-8134a0495e3c.png) <br/>
![image](https://user-images.githubusercontent.com/87578449/143689642-dfc2da64-f3b8-4937-9944-159fa5883539.png) <br/>

## *T-Tests on Suspension Coils*
When first looking at the t-test for the overall summary, the p-value comes out to exactly 1, which means we cannot reject the null hypothesis, meaning that the means are statisically similar. The same is true when specifically comparing Lot 1 whose p-value also comes out to 1. Lot 2 still has a p-value that is greater than the assumed significance level of 0.05, although it is less than 1 (0.6072 to be exact). Lot 3, however, is a different story altogether. Its p-value is 0.04168, which is less than our significance level, which means we can reject the null hypothesis; the mean for Lot 3 is statistically *different*.

![image](https://user-images.githubusercontent.com/87578449/143690328-ee0e8c6a-e50a-4e6e-860a-ebdd37a2f8ba.png)

## *Study Design: MechaCar vs. Competition*
As we head into the holiday season, it's a very popular time for consumers to buy extravagant gifts for their family members - oftentimes they go so far as to buy a brand new car for their loved ones. In order to identify if MechaCar outperforms their competition, we need to look at the top 2 factors consumers care most about: cost and reliability (ie: maintenance cost). With gas prices currently rising, we're going to add fuel efficiency as well. The null hypothesis here would be that there is no statistical difference in any of these 3 factors when comparing against other manufacturers, which means the alternative hypothesis would be that there *is* statistical difference in those 3 factors when comparing against other manufacturers. 

Because we're working with 2 samples (MechaCar and another manufacturer), we'll want to do a two-sample t-test with continuous data for our 3 metrics. We already have miles per gallon for MechaCar, but we'll need to gather pricing details and average maintenance cost per year over time. We'll need this data not only for MechaCar but for the other manufacturer(s). 

With customers eager to get into the holiday spirit, may the odds be ever in MechaCar's favor.
