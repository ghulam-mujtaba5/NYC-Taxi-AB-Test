# 🚕 NYC Yellow Taxi Fare A/B Test Analysis  
*Google Advanced Data Analytics Capstone Project – Course 4*

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-brightgreen?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?logo=matplotlib)
![Scipy](https://img.shields.io/badge/Scipy-Statistical%20Testing-lightgrey?logo=scipy)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

## 📌 Overview

This project is the capstone of Course 4 in the [Google Advanced Data Analytics Certificate](https://www.coursera.org/professional-certificates/google-advanced-data-analytics). It applies an A/B test using the **2017 NYC Yellow Taxi Trip Dataset** to determine if there's a statistically significant difference in fare amounts based on the **payment method**: credit card vs. cash.

---

## 🎯 Business Scenario

- **Client**: Automatidata  
- **Partner**: NYC Taxi & Limousine Commission (TLC)  
- **Hypothesis**: Passengers who pay by **credit card** may pay **higher fares** than those who pay **cash**.

---

## 📊 Objective

To determine whether the **average fare amount** differs significantly between:

- **Group A**: Credit Card payments  
- **Group B**: Cash payments  

---

## 🧪 Methodology

### 📂 Data Source
- [NYC TLC Trip Records (2017)](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

### 🛠 Tools & Technologies
- Python (Jupyter Notebook)
- Pandas, Numpy
- Seaborn & Matplotlib
- Scipy (Welch’s t-test)

### 🔬 Steps
1. Data loading and filtering for valid payment types and fare amounts.
2. Exploratory data analysis and visualization.
3. Conducting a **Welch’s t-test** (unequal variances).
4. Interpreting results using a significance level of α = 0.05.

---

## 📈 Results

| Group        | Mean Fare ($) | Std Dev ($) | Count   |
|--------------|---------------|-------------|---------|
| Credit Card  | **13.91**     | **9.78**    | 112,450 |
| Cash         | **11.86**     | **8.67**    | 98,532  |

- **T-statistic**: `6.87`  
- **P-value**: `6.57 × 10⁻¹²`

> **Conclusion**: We **reject the null hypothesis**.  
> **Interpretation**: There is a **statistically significant difference** in fare amounts between credit card and cash payments.  
> **Business Insight**: Riders using **credit cards** tend to pay higher fares—possibly due to ride length, tipping, or usage patterns like airport trips or business rides.

---

## 📊 Visualizations

![Fare Distribution by Payment Type](visuals/fare_distribution_plot.png)


## 📌 Key Learnings

- Applied **real-world A/B testing** on a large dataset.
- Practiced **data cleaning**, **EDA**, and **statistical testing**.
- Gained insights into **payment behavior patterns** in transportation.

---

## 📚 References

- NYC TLC Open Data: [https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- Scipy t-test docs: [https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html)
- Coursera: [Google Advanced Data Analytics Certificate](https://www.coursera.org/professional-certificates/google-advanced-data-analytics)

---

## 👨‍💻 Author

**Ghulam Mujtaba**  
BS Software Engineering | COMSATS Lahore  
[🌐 Portfolio](https://ghulammujtaba.com) | [LinkedIn](https://linkedin.com/in/ghulamujtabaofficial) | [GitHub](https://github.com/ghulam-mujtaba5)

---

## 🏁 License

This project is part of the **Coursera Google Advanced Data Analytics Certificate** coursework and is licensed for academic and portfolio use only.



