# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

-	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

According to our results, vehicle_length and ground_clearance (as well as intercept) are statistically unlikely to provide random amounts of variance to the linear model. 

-	Is the slope of the linear model considered to be zero? Why or why not?

The p-value of our linear regression analysis is 5.35 x 10-11, which is much smaller than our assumed significance level of 0.05%. Therefore, we can state that there is sufficient evidence to reject our null hypothesis, which means that the slope of our linear model is not zero.

-	Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

Yes, Multiple R-Square of 0.7149 means that vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD can explain 71% of the variation in mpg.

## Summary Statistics on Suspension Coils

-	The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

total_summary:

![total_summary](https://user-images.githubusercontent.com/92401000/152703587-540cc421-2aa5-42b2-9789-b14fbd0c0f16.PNG)

lot_summary:

![lot_summary](https://user-images.githubusercontent.com/92401000/152703659-a323ff1b-908c-40d1-857c-a69f5cfc6951.PNG)

No, the current manufacturing data DOES NOT meet this design specification for all manufacturing lots because Lot3 has a variance of 170 PSI. Only Lot1 and Lot2 meet the design specification with a variance of 0.98 and 7.5 PSI respectively.

## T-Tests on Suspension Coils

-	Determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

![all_man_lots_t test](https://user-images.githubusercontent.com/92401000/152703695-aa4f09eb-9a58-44c7-9f89-f50492c75148.PNG)

Assuming our significance level was the common 0.05 percent, our p-value=0.06028 is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

-	Determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

![lot1_t test](https://user-images.githubusercontent.com/92401000/152703710-b8be9a2b-fd51-4b10-aec4-292d0935e949.PNG)

Lot1: Assuming our significance level was the common 0.05 percent, our p-value=1.0 is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

![lot2_t test](https://user-images.githubusercontent.com/92401000/152703733-2c89e765-3f8d-4c59-9e55-1a0275b03cc2.PNG)

Lot2: Assuming our significance level was the common 0.05 percent, our p-value=0.6072 is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

![lot3_t test](https://user-images.githubusercontent.com/92401000/152703748-78907c69-af66-42fd-a0b7-38189b6aa779.PNG)

Lot3: Assuming our significance level was the common 0.05 percent, our p-value=0.04168 is below our significance level. Therefore, we do have sufficient evidence to reject the null hypothesis, and we would state that the two means are not statistically similar.

## Study Design: MechaCar vs Competition

A statistical study that quantifies how MechaCar performs against the competition would be testing the maintenance cost against its competitors. 

The null hypothesis would be there is no statistical differences between the observed sample mean (maintenance cost) and its presumed population mean (maintenance cost).

The alternative hypothesis would be there is statistical differences between the observed sample mean (maintenance cost) and its presumed population mean (maintenance cost).

We would run the One-Sample t-Test to test the hypothesis because we want to determine if there is a statistical difference between the mean of the sample distribution and the mean of the population distribution. 

The data we would need to run this statistical test would be the cost of all maintenance performed on MechaCar and its competitors. This includes the cost for oil change, tire rotations, air filters, engine fluids and car battery replacements, and so forth.
