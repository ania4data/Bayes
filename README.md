# Bayes

On Navive Bayes, tested multiple distribution 
- Cuachy, beta, weibull_min did not work out, beta after fitting for alpha and beta only gave 10% accuracy, more like random selection of 10% within 10 class
- putting constant alpha/beta, putting variables as mean and var of columns also did not workout
- rescaled the scale to 1.2, and move center to loc=-0.1  to make sure logpdf not going to infinity but did not help the accuracy. Cauchy got about max 0.4 accuracy.
- Best is gaussian since is not unoform and and we have majority of population zero give some weight to the middle of population
- Non-naive got to 0.9 with cov matrix.
