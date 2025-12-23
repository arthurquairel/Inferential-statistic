# Statistical Analysis & Hypothesis Testing Labs 📊

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![SciPy](https://img.shields.io/badge/SciPy-Statistics-blue?style=flat&logo=scipy)
![NumPy](https://img.shields.io/badge/NumPy-Computing-blue?style=flat&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=flat&logo=matplotlib)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📖 Overview

This repository contains a comprehensive statistical study divided into four main parts. The project explores fundamental statistical theorems through simulation and applies rigorous hypothesis testing to both historical biological data and clinical trial results.

The work ranges from verifying the **Central Limit Theorem (CLT)** using synthetic data to analyzing **Galton's height dataset** and evaluating the efficacy of a **Cholesterol treatment** via randomized control trial data.

---

## 📂 Project Structure

The analysis is implemented in a single Python script (`TP-STAP_Quairel.py`) covering the following modules:

### 1. The Central Limit Theorem (CLT)
* **Simulation:** Generation of synthetic random variables to demonstrate convergence towards a Gaussian distribution.
* **Analysis:** Visualization of the impact of sample size ($N$) and number of simulations ($M$) on the estimator's variance and distribution shape.

### 2. Confidence Intervals (CI)
* **Normal Distribution:** Construction of CIs when the population variance is known ($Z$-score).
* **Student's t-Distribution:** Construction of CIs for small samples where variance is unknown (Student's $t$).
* **Visualization:** Plotting rejection zones and acceptance regions for $\alpha = 0.05$.

### 3. Analysis of Galton's Height Data
* **Dataset:** Analysis of `dataA.txt` containing heights of parents.
* **Descriptive Statistics:** Calculation of biased/unbiased estimators for mean, variance, skewness, and kurtosis.
* **Normality Tests:**
    * **Chi-square Goodness-of-Fit:** Comparing empirical histograms to theoretical Gaussian distributions.
    * **Henry's Line (Q-Q Plot):** Visual assessment of normality.
* **Comparative Tests:**
    * **Fisher's F-test:** Testing for homogeneity of variances between fathers and mothers.
    * **Welch's t-test:** Testing for equality of means with unequal variances.

### 4. Clinical Trial Analysis (Cholesterol)
* **Context:** Randomized double-blind study (Treatment vs. Placebo) on 1719 patients.
* **Homogeneity Checks:**
    * **Z-test:** Proportion difference for gender balance.
    * **Chi-square Test:** Independence test for age distribution.
* **Efficacy Analysis:** One-tailed Z-test to determine if the cholesterol reduction is statistically significant compared to the placebo.

---

## 🛠 Technologies & Libraries

* **Python 3.x**
* **NumPy:** Data manipulation and random sampling.
* **Matplotlib:** Histograms, Q-Q plots, Boxplots, and Confidence Interval visualization.
* **SciPy (`stats`):** PDF/CDF functions, t-tests, Chi-square tests, and statistical computations.

---

## 🚀 Installation & Usage

### Prerequisites
Ensure you have the required libraries installed:

```bash
pip install numpy matplotlib scipy
