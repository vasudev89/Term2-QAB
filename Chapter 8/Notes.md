# Estimating the Population mean using the z statistic(sigma known)

### Fundamental Problem
- Population Sizes might be too big: infeasible to capture each element in order to calc the **mean**
- #### Examples
	> Estimating the average age of employees in a global company of 6000 employees
	>
	> Estimating the shelf life of loaves of bread

### Solution
- Take a random sample from the population and estimate the mean accordingly
<br>

### Point Estimate
- *A __point estimate__ is a __statistic__ taken from a sample that is used to estimate a __population parameter__.*
- If other random samples are drawn from the population the point estimate will show variation.

### Interval Estimate
- *An interval estimate (confidence interval) is a range of values within which the analyst can declare, with some confidence, the population parameter lies*
- May be two or one sided
<br>

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
     style="margin: auto;" />

- For 95% confidence, alpha = .05 and alpha2 = .025.
- The value of z-alpha.025 is found by looking in the standard normal table under .5000 - .0250 = .4750
- Corresponding value is 1.96

> __Common Confidence Values__: 99%, 98%, 95%, 90%. Associated z-values in table below

<img src="https://github.com/vasudev89/Term2-QAB/blob/master/Chapter%208/Table%208.1.PNG"
     alt="Table 8.1"
     style="margin: auto;" />

> Given
>
> xbar = 510, sigma = 46, n = 85, and confidence level = 95%
> 
> CF Level = 95% => z = 1.96
>
> Thus 510 - 1.96 * 46/sqrt(85) <= mu <= 510 + 1.96 * 46/sqrt(85)
>
> 500.22 <= mu <= 519.78

<br>

### Finite Correction Factor

- If the sample is taken from a finite population, a finite correction factor may be used to increase the accuracy of the solution.
- Formula will revise to
> x̅ - (z-alpha2 * σ/sqrt(n)) * sqrt((N-n)/(N-1)) <= μ <= x̅ + (z-alpha2 * σ/sqrt(n)) * sqrt((N-n)/(N-1))

- Question:
	- A study is conducted in a company that employs 800 engineers. A random sample of 50 engineers reveals that the average sample age is 34.3 years. Historically, the population standard deviation of the age of the company’s engineers is approximately 8 years. Construct a 98% confidence interval to estimate the average age of all the engineers in this company.

> Given
>
> N = 800, n = 50, sigma = 8, xbar = 34.3, CF Level = 98%
>
> For CF Level = 98%, z = 2.33
>
> Thus
> 34.3 - 2.33 * 8/sqrt(50) * sqrt((800-50)/(800-1)) <= mu <= 34.3 - 2.33 * 8/sqrt(50) + sqrt((800-50)/(800-1))
> 
> 31.75 <= mu <= 36.85
>
> __Without the correction factor, the confidence interval would be__
> 31.66 <= mu <= 36.94
>