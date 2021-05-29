# MechaCar Statistical Analysis

## Linear Regression to Predict MPG
A line called a regression line or Linear Regression is the correlation between two variables where one is dependent and the other is an independent variable. the equation y = mx + c is a straight line where the values of y are estimated from x values. When corresponing values of two (2) variables are plotted with scatter plots, we tend to find the best straight line that will fit or show the trend of input (independent) and output (dependent) values. This represents a rough correlation between the each input and output. The degree of correlation is representented by the quatity the Coefficent of Correlation. In the summary output, each Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model. The lower the value of Pr(>|t|), the less likely there will be any will be any amount of significant variance to the linear model, Linear Regression y = mx + c
Figure 1 show the the generated summary statistis![Fig1](https://user-images.githubusercontent.com/78861458/120042539-449e5380-bfd8-11eb-8705-bafb9353b642.png)

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
- Vehcile_Length
- Vehcile_weight
- ground_clearance

### Is the slope of the linear model considered to be zero? Why or why not?
The r-squared (r2) value is also known as the coefficient of determination and represents how well the regression model approximates real-world data points. The r-squared value range from 0 to 1, with 1 being the slope with the gradient of 1. The R-squared value from the Generated Summary is 0.7179 which is high so it is considered a linear model.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
The Pearson correlation coefficient is denoted as "r" in mathematics and is used to quantify a linear relationship between two numeric variables. The Pearson correlation coefficient ranges between -1 and 1. -1 simply means the graph (line) slopes to the left (ideal negative correlation) and 1 means the line slope to the right (ideal positive correlation) Idealy the closer the slope of the line is 1 the more accurately will be prediction of the outputs (dependent variabls). As per the Pearson correlation coefficient table valves of 0.70 and above are strong correlation strengh. The the adjusted R value is 0.6825 approximately 0.70.

## T-Tests on Suspension Coils
The Total Summary Dataframe is shown in figure 2, represents the overall performace of the three Lots that produces the suspesion coils. From figure 2, the two most important values are the variance and standard deviation (SD). Standard deviation is probabaly the most valuable and widely used as a measure of dispersion. This a reference of how tightly or far the samples are from the mean (average) value, in this case, "PSI" for the suspension coils. The greater the SD number the more variability of the bell curve is
and it will much wider.
Figure 2
![Fig2](https://user-images.githubusercontent.com/78861458/120050140-48d36c80-bfea-11eb-96b5-6da5864ec85d.png)

Screen shot shown in figure 3 of the lot_summary, gives separate production of the suspension coils between the 3 lots, Lot1, Lot2 and Lot3. Both the Mean and Median are almost the same but, variance and SD show significant differences.
Figure 3
![Fig3](https://user-images.githubusercontent.com/78861458/120051590-3c054780-bfef-11eb-8e3b-84e5e43ce2b6.png)

### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
The wider the bell curve the larger the standard deviation values. The current manufacturing data for all the lots, together, does not meet the design specification due to the value of both variance and standard deviation. Lot_summary dataframe, using the groupby() function, shows the Lot1 variance and SD approximatly equal to 1, the value of the SD 7.89 in the total_summary dataframe proves that specification was not met. Results of the 3 lots are as follows:

- Lot1 specfications are met, low variance and SD values
- Lot2 slightly improvment is required SD value at 2.73
- Lot3 this main cause why the manufactoring lots are not up specfication the SD value is 13.05

## T-Tests on Suspension Coils
### An RScript is written for t-test that compares all manufacturing lots against mean PSI of the population, Figure 4
![Fig4](https://user-images.githubusercontent.com/78861458/120070881-a7d0ca00-c05a-11eb-9a33-27e426b3990a.png)

### An RScript is written for three t-tests that compare each manufacturing lot against mean PSI of the population (10 pt) figure 5
![Fig5](https://user-images.githubusercontent.com/78861458/120071678-680be180-c05e-11eb-98cd-94c331a2587d.png)

### Summary of the t-test results across all manufacturing lots and for each lot.
 In the first RScript, ramdom samples taken from the Suspension Coil dataframe, tested against the entire Suspension Coil dataframe (population), statisfies the five assumptions when it comes to the one-sample t-test. The p-value = o.5297, determined from this RScript, is above the normal significant level, therefore we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar. More importantly the variance between the two dataframe will be the same if the ramdom sample are a reflection of the entir data set.
 
 Lot3, which is the production line that does not meet the manufactoring requirements, it's p-value 0.1549, is above normal significant level and null hypothesis suggest that it is simialr to the population dataframe. However, Lot1 and Lot2, p-values 9.35e-12 and 0.0005082 respectively, are below the significant level, you would have sufficient evidence to reject the null hypothesis and state that the two means are statistically different. This explains further that Lot3 is not meeting the production standard which has affected the overall performance of the factory. 





