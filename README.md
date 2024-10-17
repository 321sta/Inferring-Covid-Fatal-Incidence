# Practical-2
## Global purpose
# We aim to use the real daily death counts and model infection duration with a log-normal distribution to 
# simulate the initial infection time (t0) for each individual. The "deconv" function iteratively refines t0 
# by introducing random moves. It evaluates these changes using p_value, a modified Pearson statistic 
# that measures the discrepancy between actual and simulated death counts, to decide whether to accept the change.
# After obtaining a converged t0, we reapply the "deconv" function to quantify uncertainty in the estimated incidence 
# trajectory by assuming the observed death counts are estimates of the expected values of Poisson-distributed variables.
# Finally, we generate a plot showing the estimated incidence trajectory over time, including uncertainty visualization, 
# the observed death counts, and the date of the first UK lockdown.
