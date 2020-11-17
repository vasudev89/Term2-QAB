# Estimating the Population mean using the z statistic(sigma unknown)

### Fundamental Problem
- Population Sizes might be too big: infeasible to capture each element in order to calc the **mean**
- #### Examples
	> Estimating the average age of employees in a global company of 6000 employees
	>
	> Estimating the shelf life of loaves of bread

### Solution
- Take a random sample from the population and estimate the mean accordingly
\
\
\

### Point Estimate
- *A __point estimate__ is a __statistic__ taken from a sample that is used to estimate a __population parameter__.*
- If other random samples are drawn from the population the point estimate will show variation.

### Interval Estimate
- *An interval estimate (confidence interval) is a range of values within which the analyst can declare, with some confidence, the population parameter lies*
- May be two or one sided
\
\
\

### Confidence Interval Construction
- From Central Limit Theorem (n>=30 or the sample is normally distributed for n<30)
> z = (x̅ - μ) / (σ/sqrt(n))
- OR
> μ = x̅ - (z * σ/sqrt(n))
- Because the sample mean can be > or < than the sample mean
> μ = x̅ +/- (z * σ/sqrt(n))
#### Formal Definition
> x̅ - (z-alpha2 * σ/sqrt(n)) <= μ <= x̅ + (z-alpha2 * σ/sqrt(n))
- alpha = region in the bell curve that lies outside of the confidence interval
- alpha2 = region in the bell curve that lies outside of the confidence interval on either side(1 tail)

<img src="https://github.com/vasudev89/Term2-QAB/blob/master/Chapter%208/Fig%208.3.PNG"
     alt="Fig 8.3"
     style="float: left; margin-right: 10px;" />
<<<<<<< HEAD

> __Common Confidence Values__: 99%, 98%, 95%, 90%

