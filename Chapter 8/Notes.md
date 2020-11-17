# Estimating the Population mean using the z statistic(sigma unknown)

### Fundamental Problem
- Population Sizes might be too big: infeasible to capture each element in order to calc the **mean**
- #### Examples
	> Estimating the average age of employees in a global company of 6000 employees
	>
	> Estimating the shelf life of loaves of bread

### Solution
- Take a random sample from the population and estimate the mean accordingly

### Point Estimate
- *A __point estimate__ is a __statistic__ taken from a sample that is used to estimate a __population parameter__.*
- If other random samples are drawn from the population the point estimate will show variation.

### Interval Estimate
- *An interval estimate (confidence interval) is a range of values within which the analyst can declare, with some confidence, the population parameter lies*
- May be two or one sided

### Confidence Interval Construction
- From Central Limit Theorem (n>=30 or the sample is normally distributed for n<30)
- z-score = (x̅ - μ) / (σ/sqrt(n))
