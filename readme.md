## Analysis into the Difference in Medical procedure charges throught out the United States.

 <br/>

**The United States has some of the highest health care cost, and just how high is not consistent throughhtout the United States.**

 <br/>

The origin of the cost inflation is often a debated and often anecdotal evidence points excess bureaucracy, obesity rates, or lack of private Insurance regulation. However, the data does not seem to support these answers

 <br/>

In this project I explore medicare procedure charges throught the US states and Puerto Rico. and introduce census data features in order to try to explain the difference in medical procedure pricing from region to region.

 <br/>

## Understanding and Profiling the Data
 <br/>

#### Medical Procedur data
* 2014 full year
* All 50 States & Puerto Rico
* 12 features
* 202070 observations
* provider level data
#### Census data
* 2014 full year
* All 50 States & Puerto Rico
* 500+ features
* 33200 observations
* zip code level data

 <br/>

## Data filter & reduction methodology

<br/>

Sorted procedures by frequency and then descending price subsetting a segment of the data conatining 5 medical procedures of similiar pricing and frequency.

Reduce census data to only relevant features that represent differnce in cost of living, with the key variable being median income and control variables such as percent of the local population with medical coverage and percent of the populatin living below the poverty line.

**data was left joined on medicare data by the zipcode to retain medical procedure level data**

![image](https://github.com/miguelangel22/MedicalProcedurePricing/blob/master/img/Most%20Expensive%20Common%20Procedures.png)

<br/>

![image](https://github.com/miguelangel22/MedicalProcedurePricing/blob/master/img/Regression%20of%20Log%20Price%20Median%20Income.png)

## Inferential Regression analysis

* The residuals appear to be Homoscedastic
* clusters with similar/ constant variance
* Small outliers and Leverage points

![image](https://github.com/miguelangel22/MedicalProcedurePricing/blob/master/img/Residual%20plot.png)

<br/>

* Residuals follow a normal distribution with a small degree of right smaller degree of right skewness after taking the log transformation.

* Whether my data is Independent and identically Distributed is debatable.

* Information about the collection methods utilized by Census & Medicare can be found on my GitHub page.

![image](https://github.com/miguelangel22/MedicalProcedurePricing/blob/master/img/QQ%20Plot.png)

<br/>

## Summary and Implications

* My Analysis on the source of difference in medical procedure pricing is inconclusive.

* However there is still many insightful implications to walk away with from this presentation

* The fact that the signals from the model were weak it  is an implication on its own.

* Further analysis and data collection on provider level medical practice difference, real economic incentives of providers and business structure of providers can provide further insight.

