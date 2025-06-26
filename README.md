

# Two-Sample t-Test – Python Coding Test (10 Questions)

## Instructions:

* Answer each question using Python.
* You may use libraries like `scipy.stats`, `pandas`, or `numpy`.
* Each question tests understanding of two-sample t-tests: assumptions, application, and interpretation.

---

## Question 1: Basic Test

You are given two groups of exam scores:

```python
group1 = [85, 87, 88, 90, 86]
group2 = [82, 83, 85, 81, 84]
```

Perform a two-sample t-test and report the **t-statistic** and **p-value**.

---

## Question 2: Equal vs Unequal Variance

Use the same data from Question 1.

Perform the test **assuming unequal variances** (`equal_var=False`). What changes?

---

## Question 3: Interpret the Results

Interpret the result from **Question 2** in simple language. What does the p-value mean?

---

## Question 4: Use Real Data (Heights)

```python
import pandas as pd

data = {
    'gender': ['M', 'M', 'F', 'F', 'M', 'F', 'M', 'F', 'F', 'M'],
    'height': [175, 180, 165, 160, 178, 163, 182, 164, 162, 179]
}
df = pd.DataFrame(data)
```

Use a two-sample t-test to test whether **male and female heights** differ significantly.

---

## Question 5: Visualize the Data

Use the height data above.

Plot **boxplots** for male and female heights to visualize the difference. (Use `matplotlib` or `seaborn`.)

---

## Question 6: Check Assumptions

For the height data in Question 4:

* Test for **normality** (use `scipy.stats.shapiro`)
* Test for **equal variances** (use `levene` or `bartlett` test)

---

## Question 7: Simulate and Test

Create two normally distributed datasets:

```python
import numpy as np

groupA = np.random.normal(50, 5, 30)
groupB = np.random.normal(55, 5, 30)
```

Test if group means differ significantly.

---

## Question 8: One-Tailed vs Two-Tailed Test

Modify the test in Question 7 to check:

* Whether **groupA < groupB** using a **one-tailed test**.
* What do you conclude?

---

## Question 9: Use a CSV File

Use a CSV dataset from the link below:

📄 [https://people.sc.fsu.edu/\~jburkardt/data/csv/airtravel.csv](https://people.sc.fsu.edu/~jburkardt/data/csv/airtravel.csv)

* Read the data using `pandas`
* Compare January and February passenger counts across years using a **two-sample t-test**

---

## Question 10: Report Like a Scientist

Using **any one test above**, write a short report:

* State the null and alternative hypotheses.
* Mention t-stat, p-value.
* Conclusion (in plain language).

