Presentation.Rproj
========================================================
author: FreelancerAlpha1-1
date: July 2014

First Slide
========================================================

For more details on authoring R presentations click the
**Help** button on the toolbar.

Linear Regression Model on mtcars

Presenting simple linear regression between MPG as outcome and others as predictors
Basic Model: y= b0 + b1x1 + b2x2 +.+bpxp + ei; i= 1 n

Second Slide
========================================================
## Regarding Ui.r

1. Ui.R is having code to show the select box for independent variable
2. User can select any option from select box to create model 
3. select element is reactive and will pass the input to server as per user's actions.
4. Dependent variable is fixed and cannot be changed.

--- .class #id

Third Slide
========================================================
## Regarding server.r

1. server.R is having code to create the model from the reactive input
2. Server.R will accept the input as independent variable and will create model 
3. This also uses the helpers.R file, where model creation function is defined.
4. It provides the reactive output variables to UI.R to display various plots.

--- .class #id

Fourth Slide
========================================================
## helpers.R and model

1. This has function which creates model for server.R
2. It accepts input variable as independent variable.
3. it goes through various statements and select appropriate variable to create model.

Fifth Slide
========================================================
## Outputs

1. Output will show the various model plot
2. Residual vs Fitted
3. Normal Q-Q
4. Scale-Location
5. Cook's Distance
6. Residuals vs Leverage
7. Cook's Distance vs Leverage.
8. Next is an example of a model of mpg as outcome and wt as predictor.

--- .class #id

Slide With Code
========================================================


```r
summary(cars)
```

```
     speed           dist    
 Min.   : 4.0   Min.   :  2  
 1st Qu.:12.0   1st Qu.: 26  
 Median :15.0   Median : 36  
 Mean   :15.4   Mean   : 43  
 3rd Qu.:19.0   3rd Qu.: 56  
 Max.   :25.0   Max.   :120  
```

Slide With Plot
========================================================

![plot of chunk unnamed-chunk-2](Presentation.Rproj-figure/unnamed-chunk-2.png) 
