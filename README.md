# MechaCar_Statistical_Analysis

The new MechaCar from AutosRUs is "suffering from manufacturing issues," and the business is hoping that an analytical assessment will shed some light on the situation. This project's objective is to

* determine the factors that influence the MPG of car prototypes;
* Compile summary data on the suspension coils' PSI;
* assess if statistical differences between manufacturing lots and the mean population exist;
* create a research to assess how the MechaCar performs in comparison to other models.

## Deliverable 1: MPG Prediction Using Linear Regression

50 prototype MechaCars' mpg test results are included in the MechaCar mpg.csv dataset. Multiple design criteria were used to create the MechaCar prototypes in order to determine the perfect vehicle performance. We will create a linear model in R that makes use of a number of factors and coefficients to forecast the mpg of MechaCar prototypes.


## 1. Using linear regression

Using the script to calculate the linear regression we get the below coefficients.

![Linear Regression PNG](https://user-images.githubusercontent.com/23088053/217231773-67809856-04c0-48bb-9c9d-f83cdf01d0eb.png)

Vehicle length and ground clearance are the most important factors in the dataset that have a non-chronological impact on MechaCar`s MPG.
A linear regression model comparing these factors with the MPG data yielded p-values of 2.6 x 10-12 and 5.21 x 10-8, respectively, as indicated by the yellow arrows in the image above.

![Summary Linear Regression PNG](https://user-images.githubusercontent.com/23088053/217231708-71517ade-532c-4f8b-aa4b-17244b68eb04.png)

## Predictions for linear regression
All variables/coefficients are directly proportional to the mpg value, so the slope of the linear model is not considered zero.The linear model does not effectively predict the mpg of his MechaCar prototype as the multiple linear regression p-value is 5.35e-11, which is higher than 0.05 and not significance.

## Summary Statistics 

Continuous PSI Variables for Suspension Coils Across All Production Lots
The total_summary in the table below shows the mean, median, variance, and SD of his PSI for suspension coils across all manufacturing units, with suspension coil variances less than 100 PSI.

![Output 1](https://user-images.githubusercontent.com/23088053/217233002-0fda8783-8150-4ff1-85f8-4462fc70efa6.png)

![Output 2](https://user-images.githubusercontent.com/23088053/217232934-18eb0b17-5f46-4198-9e1c-d8951dfd67d3.png)

## T-Tests on Suspension Coils
For each R, the suspension coil distribution satisfies the Lot1, Lot2, and Total design constraints. However, Los3 alone exceeds 100 and does not meet the specification (exact number:170.2861224) Pounds per square inch variance. 

![t_test PNG](https://user-images.githubusercontent.com/23088053/217234017-62128c79-6c52-4c63-b18a-40a69903b751.png)

Based on the output image, t.test shows a p-value of 0.06028 for PSI for all production lots, with a statistical difference between the data set mean and the popula
tion mean It shows that there is good and strong evidence that The p-values for Lot1 and Lot2 are 1 and 0.6072, respectively.
![t_test_lot1 PNG](https://user-images.githubusercontent.com/23088053/217234068-6a87afed-896c-430b-9ed0-35aeb7bf506a.png)
![t_test_lot2 PNG](https://user-images.githubusercontent.com/23088053/217234167-5c19d6cf-ee7f-4c73-8523-2652775ead83.png)
![t_test_lot3 PNG](https://user-images.githubusercontent.com/23088053/217234346-dc2a241d-c2cf-4669-8c98-0d2e50afe0e2.png)

## Changes and results

highway fuel efficiency, horsepower, maintenance costs, seating capacity, PSI, mpg, ground clearance, fuel type, safety rating, etc.
You can test highway fuel economy, performance and cost.
These metrics are directly proportional, so you can justify the cost of your vehicle compared to your competitors.2.
The null hypothesis is the statement that there is no difference between the sample mean or proportion and the population mean or proportion.
Since we are comparing two population means, we can use a 2-sample t-test.
I also want to know if one population mean is greater or less than the other, so I can do a one-tailed t-test.
