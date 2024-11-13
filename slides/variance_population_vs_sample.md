---
marp: true
theme: default
paginate: true
---

# Understanding Variance

**Population vs. Sample Variance**

---

## Population Variance

**Definition:** Measures the average squared deviation from the population mean.
**Formula:**
$$\sigma^2 = \frac{\sum_{i=1}^{N} (x_i - \mu)^2}{N}$$

$N$: Total number of observations
$x_i$: Each observation
$\mu$: Population mean

---

## Sample Variance

**Definition:** Estimates the population variance from a sample.
**Formula:**
$$
s^2 = \frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n - 1}
$$

$n$: Sample size
$x_i$: Each observation in the sample
$\bar{x}$: Sample mean

---

## Why Use $n - 1$ in Sample Variance?

**Bessel's Correction:** Adjusts for the bias in estimating the population variance.

**Purpose:** Provides an unbiased estimator by accounting for the degrees of freedom lost when estimating the mean.

---

## Proof of Unbiasedness

**Objective:** Show that $E[s^2] = \sigma^2$.

---

## Proof (Part 1)

- Start with the sample variance formula:
  $$
  s^2 = \frac{1}{n-1} \sum_{i=1}^{n} (x_i - \bar{x})^2
  $$
- Expand $(x_i - \bar{x})^2$:
  $$
  (x_i - \bar{x})^2 = (x_i - \mu + \mu - \bar{x})^2
$$

---

## Proof (Part 2)

- Simplify the expanded form:
  $$
  (x_i - \bar{x})^2 = (x_i - \mu)^2 + 2(x_i - \mu)(\mu - \bar{x}) + (\mu - \bar{x})^2
  $$
- Sum over all observations and take expectations.

---

## Proof (Part 3)

- Utilize properties of expectations:
  $$
  E[(x_i - \mu)^2] = \sigma^2
  $$
  $$
  E[(\mu - \bar{x})^2] = \frac{\sigma^2}{n}
  $$
- Combine results to show:
  $$
  E[s^2] = \sigma^2
  $$

---

## Conclusion

- The sample variance $s^2$ is an unbiased estimator of the population variance $\sigma^2$.
- Using $n - 1$ in the denominator corrects the bias inherent in sample estimates.

