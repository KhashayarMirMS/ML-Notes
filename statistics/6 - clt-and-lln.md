# Previous
[Normal Approximation](./5%20-%20normal%20approximation.md)

## Parameter and statistic (review)
`Parameter` is a quantity of interest about the population and statistic is the the quantity measured in a sample, which will be our estimate of the parameter.

$\mu$ and $\sigma$ are the population average and standard deviation while $\bar{x}$ and $s$ are the average and standard deviation of the sample.

If we do a random draw we expect the value to be around $\mu$, give or take $\sigma$.

The `standard error (SE)` of a statistic tells roughly how far the the statistic will be from its expected value. It plays the same role that the standard deviation plays for one observation drawn at random.

# The square root law
$$SE(\bar{x}) = \frac{\sigma}{\sqrt{n}}$$

- This shows that the standard error becomes smaller if we use a larger sample size `n`. We can use this formula to determine what sample size is required for a desired accuracy.
- The formula **does not depend on the size of the population**, only the size of the sample.

# Expected value for $\bar{x}$ and sum
$$E(\bar{x}) = \mu$$

If we are interested in the sum of `n` draws $S_n$:
$$S_n = n\bar{x} \Rightarrow$$
$$E(S_n) = n \times E(\bar{x}) = n\mu$$
$$SE(S_n) = n \times SE(\bar{x}) = \sqrt{n}\sigma$$

So the variability of $S_n$ increases at the rate $\sqrt{n}$

# Law of Large Numbers
The square root law says that $SE(\bar{x}_n)$, goes to zero as the sample size increases. So if the sample size is large enough, $\bar{x}$ is close to $\mu$. This is called the `law of large numbers`.

This applies
- For average and therefore percentages but not for sums, as their standard deviation increases.
- For sampling with replacement from a population or for simulating data from a probability histogram.

More advanced versions of the LLN state that the empirical histogram of the data will be close to the probability histogram. 

# Central Limit Theorem
When sampling with replacement and `n` is large enough, the sampling distribution of the sample average (or sum or percentage) approximately follows the normal curve. So we can use normal approximation for them.

For the normal approximation to work the key requirements are:
- We sample with replacement, or simulate independent random variables from the same distribution.
- The statistic of interest is a sum (averages and therefore percentages are sums in disguise).
- The sample size is large enough: More skewed population histogram, requires large sample size.