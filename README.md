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
