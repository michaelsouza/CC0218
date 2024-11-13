---
marp: true
theme: default
class: lead
paginate: true
---

# Properties of Variance

**Understanding Variance in Statistics**

---

## 1. Definition of Variance

- **Variance ($\sigma^2$)**
  - Measures the **spread** of a set of numbers.
  - Formula:
    $$
    \sigma^2 = \frac{1}{n} \sum_{i=1}^{n} (X_i - \mu)^2
    $$
  - Where:
    - $X_i$ = each value
    - $\mu$ = mean of the values
    - $n$ = number of values

---

## 2. Non-Negativity

- **Variance is Always Non-Negative**
  - $\sigma^2 \geq 0$
  - *Reason*: Squared deviations are always positive or zero.

- **Interpretation**
  - A variance of **0** indicates no spread; all values are identical.
  - Higher variance indicates more spread out data.

---

## 3. Scaling Property

- **Variance and Scaling**
  - For a constant $c$:
    $$
    \text{Var}(cX) = c^2 \cdot \text{Var}(X)
    $$
  - *Implication*: Scaling a random variable by $c$ scales its variance by $c^2$.

- **Example**
  - If $X$ has variance 4, then $3X$ has variance $9 \times 4 = 36$.

---

## 4. Additivity for Independent Variables

- **Variance of Sum of Independent Variables**
  - If $X$ and $Y$ are independent:
    $$
    \text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y)
    $$
  - *Implication*: Variances add up when variables are independent.

- **Note**
  - If $X$ and $Y$ are **not** independent, covariance must be considered:
    $$
    \text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y) + 2\text{Cov}(X, Y)
    $$

---

## 5. Variance of a Constant

- **Variance of a Constant is Zero**
  - For any constant $c$:
    $$
    \text{Var}(c) = 0
    $$
  - *Reason*: There is no deviation from the constant value.

---

## 6. Relationship with Standard Deviation

- **Standard Deviation ($\sigma$)**
  - Square root of variance:
    $$
    \sigma = \sqrt{\sigma^2}
    $$
  - **Interpretation**:
    - Same units as the original data.
    - More interpretable in the context of the data's scale.

---

## 7. Alternative Formulas for Variance

### 7.1. Alternative Formula Using Expected Values

- **Population Variance**
  $$
  \sigma^2 = E[X^2] - (E[X])^2
  $$
  - **$E[X]$**: Expected value (mean) of $X$
  - **$E[X^2]$**: Expected value of $X^2$

- **Sample Variance**
  $$
  s^2 = \frac{\sum_{i=1}^{n} X_i^2 - \frac{(\sum_{i=1}^{n} X_i)^2}{n}}{n - 1}
  $$
  - *Derivation*:
    $$
    \text{Var}(X) = E[X^2] - (E[X])^2
    $$
    For a sample:
    $$
    s^2 = \frac{1}{n - 1} \left( \sum_{i=1}^{n} X_i^2 - \frac{(\sum_{i=1}^{n} X_i)^2}{n} \right)
    $$

---

## 7.2. Sum of Squares Formula

- **Population Variance**
  $$
  \sigma^2 = \frac{\sum_{i=1}^{N} X_i^2}{N} - \mu^2
  $$

- **Sample Variance**
  $$
  s^2 = \frac{\sum_{i=1}^{n} X_i^2 - \frac{(\sum_{i=1}^{n} X_i)^2}{n}}{n - 1}
  $$

- **Usage**
  - Often used in statistical software and computational algorithms for numerical stability and efficiency.

---

## 7.3. Using Covariance

- **Variance as Covariance**
  $$
  \text{Var}(X) = \text{Cov}(X, X)
  $$

- **Implication**
  - Useful in multivariate statistics and when dealing with multiple variables simultaneously.

---

## 7.4. Welford's Online Algorithm

<div style="display: flex; justify-content: space-between;">
<div style="width: 48%; border: 2px solid #ccc; border-radius: 10px; padding: 15px;">

$n = 0;\quad \mu_0 = 0;\quad y_0 = 0$

**For each new data point** $X_i$:
$\quad n = n + 1$
$\quad \delta = X_i - \mu_{n-1}$
$\quad \mu_n = \mu_{n-1} + \delta / n$
$\quad y_n = y_{n-1} + \delta \times (X_i - \mu_n)$

$s^2 = y_n / (n - 1)$
$\sigma^2 = y_n / n$
</div>
<div style="width: 48%;">

- **Advantages**:
  - **Memory Efficiency**: Only stores current mean and $y$.
  - **Numerical Stability**: Reduces numerical errors compared to sum of squares.

</div>
</div>

---

## 7.5. Variance in Terms of Deviation Scores

- **General Formula**
  $$
  \text{Var}(X) = \frac{1}{N} \sum_{i=1}^{N} (X_i - a)^2 - (E[X] - a)^2
  $$
  - **$a$**: Any constant

- **Note**
  - Variance is minimized when $a = \mu$ (the mean).

---

## 7.6. Matrix Form for Multivariate Data

- **Covariance Matrix ($\Sigma$)**
  $$
  \Sigma = 
  \begin{bmatrix}
  \text{Var}(X_1) & \text{Cov}(X_1, X_2) & \dots & \text{Cov}(X_1, X_p) \\
  \text{Cov}(X_2, X_1) & \text{Var}(X_2) & \dots & \text{Cov}(X_2, X_p) \\
  \vdots & \vdots & \ddots & \vdots \\
  \text{Cov}(X_p, X_1) & \text{Cov}(X_p, X_2) & \dots & \text{Var}(X_p) \\
  \end{bmatrix}
  $$

- **Usage**
  - Essential in multivariate statistics, Principal Component Analysis (PCA), and other multivariate techniques.

---

## 7.7. Geometric Interpretation

- **Sum of Squared Distances**
  $$
  \text{Var}(X) = \frac{1}{N} \sum_{i=1}^{N} \| X_i - \mu \|^2
  $$

- **Application**
  - Useful in geometry-based statistical methods and understanding variance in higher-dimensional spaces.

---

## 8. Summary: Properties

- **Variance** is a fundamental statistical measure that quantifies data spread.
- **Key Properties**:
  - Always non-negative.
  - Scales with the square of constants.
  - Adds up for independent variables.
  - Zero for constants.
- Understanding these properties is essential for statistical analysis and probability theory.

---

## 8. Summary: Formulas

- **Alternative Formulas**:
  - **Expected Values**: $E[X^2] - (E[X])^2$
  - **Sum of Squares**: Efficient computational formulas.
  - **Covariance Relationship**: $\text{Var}(X) = \text{Cov}(X, X)$
  - **Online Algorithms**: Suitable for streaming data.
  - **Matrix Form**: For multivariate data analysis.
  - **Geometric Interpretation**: Understanding variance in multiple dimensions.
- Understanding both the properties and alternative formulas of variance enhances flexibility and efficiency in statistical analysis, probability, and inferential statistics.
    
---
<!-- _backgroundColor: orange -->
<div style="text-align: center">

# Questions?

</div>
