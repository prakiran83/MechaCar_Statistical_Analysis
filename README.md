# MechaCar_Statistical_Analysis

## Overview
The goal of this project is to help Jeremy and the data analytics team to review the production data for insights that might help MechaCar's production troubles. In order to achieve our goal, we are:
1. Performing multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes,
2. Collecting summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots,
3. Running t-tests to determine if the manufacturing lots are statistically different from the mean population, and
4. Designing a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG
![predict mpg](https://user-images.githubusercontent.com/100887673/174499484-2674c3e9-87dc-40e2-be9a-b346a49018d2.png)

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

-> The intercept, vehicle_length, and ground_clearance coeeficients can be said to provide a non-random amount of variance to the mpg values.

Is the slope of the linear model considered to be zero? Why or why not?

-> The slope is not 0 because the p-Value for this model, 5.35e-11, is much smaller than the assumed significance level of 0.05%, which indicates there is sufficient evidence to reject our null hypothesis.

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

-> This linear model does predict mpg of MechaCar's effectively. Eventhough the R-squared value drops from 0.7149 to 0.6825 (adjusted), the drop is relatively very minute. So, this does predict the mpg of the prototype effectively.

## Summary Statistics on Suspension Coils
![total_summary](https://user-images.githubusercontent.com/100887673/174500165-a17597cb-d024-44ad-a2f2-eecb4be42bd4.png)
![lot_summary](https://user-images.githubusercontent.com/100887673/174500171-2d0d563f-0f69-4207-8309-3a29159c43ce.png)

Overall, the dataset indicates that the current manufacturing data does meet the 100 pounds per Sq. inch limitation. But, individually, the 3rd lot shows a much higher variance most probably because the lots are chosen randomly.

## T-Test on Suspension Coils
![test on entire lot](https://user-images.githubusercontent.com/100887673/174500257-7606676a-2a57-447a-8be4-84377e4ce648.png)

Looking at the stats it can be said that there is not enough evidence to support rejecting the null hypothesis because the p-value of 0.06 is higher that the common significance level of 0.05.

![test on 3 lots](https://user-images.githubusercontent.com/100887673/174500281-2ac1776b-61c4-401f-976b-29710f762a17.png)

## Lot 1
-> Fail to reject null hypothesis since p-value is eqaul to 1.

-> actually has a true sample mean of 1500.

## Lot 2
-> Null hypothesis cannot be rejected.

-> Sample mean of 1500.02, similar to Lot 1.

## Lot 3
-> sample mean is 1496.14 & p-value is 0.041, both below their significant levels

-> Null hypothesis can be rejected.

## Study Design: MechaCar vs Competition

Gasoline is getting very expensive these days and any car that can provide more miles per gallon will attract a lot of customers. On top of that, customers are also looking for a car that does not cost an arm and a leg. So, i believe the focusing on the metrics below can give MechaCar an advantage in the market;
1. Cost
2. Fuel efficiency
3. Maintenance cost
4. safety

By focusing onn these, the company will be able to attract a lot of customers from various demographics. Although focusing on these 4 might mean that the car will have to negotiate on its Horse power / performance. But, I believe that the number of potential customers that will move away from the car because os the performance will be very minute.
