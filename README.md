# 🚕 NYC Yellow Taxi Fare A/B Test Analysis

A clean, reproducible analysis of whether fare amounts differ by payment method (Credit vs Cash) using the 2017 NYC Yellow Taxi dataset.

<p align="left">
  <img alt="Python" src="https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white" />
  <img alt="Jupyter" src="https://img.shields.io/badge/Made%20with-Jupyter-F37626?logo=jupyter&logoColor=white" />
  <img alt="Pandas" src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" />
  <img alt="Seaborn" src="https://img.shields.io/badge/Seaborn-Visualization-0B7285" />
  <img alt="Status" src="https://img.shields.io/badge/Project-Completed-22c55e" />
</p>

---

## 📌 Contents
- [Overview](#-overview)
- [Business Scenario](#-business-scenario)
- [Objective](#-objective)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Setup](#-setup)
- [Usage](#-usage)
- [Methodology](#-methodology)
- [Results](#-results)
- [Visualizations](#-visualizations)
- [Requirements](#-requirements)
- [References](#-references)
- [Author](#-author)
- [License](#-license)

---

## 🎯 Overview
This project is part of the Google Advanced Data Analytics Capstone (Course 4). It applies an A/B test on the 2017 NYC Yellow Taxi Trip dataset to determine if fare amounts differ by payment method.

---

## 💼 Business Scenario
- Client: Automatidata  
- Partner: NYC Taxi & Limousine Commission (TLC)  
- Hypothesis: Credit card payers may pay higher fares than cash payers.

---

## 🎯 Objective
Assess whether the average fare amount differs significantly between:
- Group A: Credit Card payments  
- Group B: Cash payments

---

## 🗂️ Dataset
- Local file: `2017_Yellow_Taxi_Trip_Data.csv`
- Source: NYC TLC Trip Records (2017): https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

---

## 🧭 Project Structure
```
NYC-Taxi-AB-Test/
├─ 2017_Yellow_Taxi_Trip_Data.csv
├─ Fare_Analysis_and_Hypothesis_Testing.ipynb
├─ README.md
└─ requirements.txt
```

---

## ⚙️ Setup
```bash
# 1) create & activate a virtual environment (recommended)
python -m venv .venv
# Windows PowerShell
. .venv\Scripts\Activate.ps1

# 2) install dependencies
pip install -r requirements.txt

# 3) start Jupyter
jupyter notebook
```

---

## ▶️ Usage
Open and run the notebook:
- `Fare_Analysis_and_Hypothesis_Testing.ipynb`

Notebook covers:
- Data loading & cleaning
- EDA & visualizations
- Welch’s t-test (α = 0.05)
- Interpretation & business insights

---

## 🧪 Methodology
1) Data Source & Filtering  
2) Exploratory Data Analysis (EDA)  
3) Welch’s t-test for mean comparison (unequal variances)  
4) Statistical conclusion at α = 0.05

---

## 📈 Results
| Group       | Mean Fare ($) | Std Dev ($) | Count   |
|-------------|----------------|-------------|---------|
| Credit Card | 13.91          | 9.78        | 112,450 |
| Cash        | 11.86          | 8.67        | 98,532  |

- T-statistic: `6.87`  
- P-value: `6.57 × 10⁻¹²`

Conclusion: Reject H0. There is a statistically significant difference in fare amounts between payment methods. Riders using credit cards tend to pay higher fares—potentially due to trip length, tipping, or patterns like airport/business trips.

---

## 📊 Visualizations
The notebook produces plots such as:
- Fare distribution by payment type
- Boxplots comparing groups
- Additional EDA visuals

Tip: Export figures to a `plots/` folder and embed them here for a richer README.

---

## 🧾 Requirements
See `requirements.txt`. Core libraries:
- pandas, numpy
- matplotlib, seaborn
- scipy
- jupyter

---

## 📚 References
- NYC TLC Open Data: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page  
- SciPy t-test docs: https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html  
- Coursera: Google Advanced Data Analytics Certificate

---

## 👨‍💻 Author
**Ghulam Mujtaba**  
Portfolio: https://ghulammujtaba.com  
LinkedIn: https://linkedin.com/in/ghulamujtabaofficial  
GitHub: https://github.com/ghulam-mujtaba5

---

## 🏁 License
Academic/portfolio use as part of the Google Advanced Data Analytics coursework.
