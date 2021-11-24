# MechaCar_Statistical_Analysis

## Project Overview

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on me team to review the production data for insights that may help the manufacturing team.

In this challenge, I helped do the following:

- Performed multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collected summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Ran t-tests to determine if the manufacturing lots are statistically different from the mean population
- Designed a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.
## Linear Regression to Predict MPG

<img width="505" alt="Screen Shot 2021-11-24 at 2 45 41 PM" src="https://user-images.githubusercontent.com/88408350/143322247-db05694e-91d2-4eef-a15c-699a62820516.png">

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The variables that provided a non-random amount of variance were vehicle weight, spoiler_angle & AWD. The two variables that had the most amount of random variance are ground_clearance and vehicle_length.

- Is the slope of the linear model considered to be zero? Why or why not?

Our slope is not zero because the p-value is less than 0.05

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

Since our R-squared value is 71.49%, this means 71.49% of the model will predict mpg values correctly. This is a pretty effective calculation, but there are still other facts that could change the data.
## Summary Statistics on Suspension Coils

<img width="542" alt="Screen Shot 2021-11-24 at 3 13 30 PM" src="https://user-images.githubusercontent.com/88408350/143324249-dfaaf047-4b4b-4bcb-a4dc-24b2e8314210.png">

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Lot 1 and Lot 2 are both within design specifications for the MechaCar suspension coils and have nearly the same exact mean and median. Lot 3 had a much higher variance and is outside of the design specifications. 

## T-Tests on Suspension Coils

**- T-test across all lots:**

<img width="412" alt="Screen Shot 2021-11-24 at 3 20 04 PM" src="https://user-images.githubusercontent.com/88408350/143324693-a37d1132-e7a7-4e5a-b0de-d41e3482b6fc.png">

Across all lots, we fail to reject the null hypothesis since the p-value equals 0.06028. Therefore, we cannot reject the fact that the sample mean may be equivalent to the true population mean. 

**- T-test on Lot 1:**

<img width="507" alt="Screen Shot 2021-11-24 at 3 19 55 PM" src="https://user-images.githubusercontent.com/88408350/143324771-609f50b5-047c-4b37-97b6-7c306fd32855.png">

For Lot 1, we fail to reject the null hypothesis since the p-value equals 1. As the p-values get larger, the confidence interval becomes smaller, so the true population mean becomes more accurate. 


**- T-test on Lot 2:**

<img width="511" alt="Screen Shot 2021-11-24 at 3 19 46 PM" src="https://user-images.githubusercontent.com/88408350/143324764-5d18042e-9fc5-4ee1-b13b-b5d6f7f912b8.png">

For lot 2, we fail to reject the null hypthesis since the p-value equals 0.6072. The second lot has a slightly smaller confidence interval.


**- T-test on Lot 3:**

<img width="519" alt="Screen Shot 2021-11-24 at 3 19 41 PM" src="https://user-images.githubusercontent.com/88408350/143324750-af6c7b39-0868-4056-b259-6ebda2db91be.png">

For lot 3, we can reject the null hypothesis since the p-value equals 0.04168. Unlike the other two lots, the confidence interval for Lot 3 does not include the predicted population mean.

## Study Design: MechaCar vs Competition

A statistical study that would be interesting to quantify to see how the MechaCar performs against the competition is a car's horespower. We can use the same tests in this analysis to see if MechaCar is much different from its competitors

- What metric or metrics are you going to test?

1. Horsepower
2. MPG 
3. Engine Size

- What is the null hypothesis or alternative hypothesis?

Null Hypothesis (Ho): There is no statistical difference between the competition's horse power dataset and MechaCar's dataset.
Alternative Hypothesis (Ha): There is statistical difference between the competition's horse power dataset and MechaCar's dataset.

- What statistical test would you use to test the hypothesis? And why?

I would use t-tests to compare the population of our data with the competitors. 

- What data is needed to run the statistical test?

At a significance level of 0.05, the data that results of a p-value smaller than 0.05 would prove that the null hypothesis could be rejected. If the Ha is true, we can predict that MechaCar has better horse power compared to their competitors. 
