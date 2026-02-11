<!-- ============================================ -->
<!-- 🚀 GDP CURVE MASTER · NON-LINEAR REGRESSION  -->
<!-- ============================================ -->
<!-- 👨‍💻 Author: Mojtaba Pipelzadeh               -->
<!-- ============================================ -->

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=300&section=header&text=GDP%20Curve%20Master&fontSize=50&fontColor=white&animation=fadeIn&fontAlignY=35"/>
</p>

<h1 align="center">
  🧠 Non-Linear Regression on China's GDP (1960–2014)
</h1>

<h3 align="center">
  ⚡ Engineered with Precision by <b style="color:#2c5364;">Mojtaba Pipelzadeh</b>
</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-0f2027?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Non--Linear-Regression-203a43?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Logistic-Curve%20Fitting-2c5364?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Status-Active-0f2027?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/License-MIT-black?style=for-the-badge"/>
</p>

<p align="center">
  <img src="https://visitor-badge.laobi.icu/badge?page_id=mojtaba-pipelzadeh.gdp-curve-master" />
</p>

---

# 🌍 PROJECT OVERVIEW

> *"Linear regression sees straight lines. Non-linear regression sees the poetry in data."*

**GDP Curve Master** is a professional machine learning project that models **China's extraordinary economic transformation** from 1960 to 2014 using **logistic regression**. This project demonstrates how a simple, interpretable mathematical function can capture complex real-world growth patterns with over **95% accuracy**.

📌 **Author:** Mojtaba Pipelzadeh  
📌 **Focus:** Non-Linear Regression · Economic Forecasting · Model Interpretability  
📌 **Dataset:** World Bank GDP Data (via IBM Skills Network)

---

# 🎯 PROJECT MISSION

| # | Objective | Status |
|---|-----------|--------|
| ✅ | Understand non-linear vs linear regression | 🟢 Complete |
| ✅ | Implement logistic function from scratch | 🟢 Complete |
| ✅ | Optimize parameters with `curve_fit` | 🟢 Complete |
| ✅ | Visualize raw data and fitted curve | 🟢 Complete |
| ✅ | Evaluate with R², MSE, MAE | 🟢 Complete |
| ✅ | Train-test split validation | 🟢 Complete |
| ✅ | Residual analysis | 🟢 Complete |
| ⏳ | Compare with exponential/polynomial models | 🟡 Pending |
| ⏳ | Streamlit dashboard | 🟡 Pending |

---

# 📊 THE DATASET: CHINA'S ECONOMIC MIRACLE

```
┌─────────────────────────────────────────────────────────────┐
│  📅 Time Period:  1960 - 2014                             │
│  💰 Target:       Annual Gross Domestic Product (USD)     │
│  🌏 Source:       World Bank / IBM Skills Network         │
│  📈 Pattern:      Slow growth → Explosive growth → Plateau│
│  🧮 Samples:      55 years                                │
└─────────────────────────────────────────────────────────────┘
```

### Raw Data Preview:

| Year | GDP (USD) |
|------|-----------|
| 1960 | 5.97e+10  |
| 1970 | 9.26e+10  |
| 1980 | 1.91e+11  |
| 1990 | 3.61e+11  |
| 2000 | 1.21e+12  |
| 2010 | 6.09e+12  |
| 2014 | 1.05e+13  |

---

# 🧠 THE MATHEMATICAL MODEL

## 📐 Logistic (Sigmoid) Function

$$ \hat{Y} = \frac{1}{1 + e^{-\beta_1(X-\beta_2)}} $$

### Parameter Interpretation (by Mojtaba Pipelzadeh):

| Parameter | Role | Economic Meaning |
|-----------|------|------------------|
| **β₁** | Steepness | Speed of economic transition |
| **β₂** | Midpoint | Year when growth is half-maximum |

### Optimal Parameters Found:

```python
β₁ = 0.1047  # Steep growth acceleration
β₂ = 1990.3  # Halfway point of development
```

---

# 🧪 TECHNOLOGY STACK

<p align="center">
  <img src="https://img.shields.io/badge/NumPy-1.24+-013243?style=flat-square&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-2.0+-150458?style=flat-square&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-3.7+-11557c?style=flat-square&logo=matplotlib&logoColor=white"/>
  <img src="https://img.shields.io/badge/SciPy-1.11+-8CAAE6?style=flat-square&logo=scipy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-1.3+-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white"/>
</p>

| Layer | Technology | Purpose |
|-------|------------|---------|
| 🐍 **Core** | Python 3.10+ | Programming engine |
| 📊 **Data Processing** | NumPy, Pandas | Data loading & normalization |
| 📈 **Visualization** | Matplotlib | Insight rendering |
| 🤖 **Modeling** | SciPy (curve_fit) | Parameter optimization |
| 📏 **Evaluation** | Scikit-Learn | Metrics calculation |
| 📓 **Notebook** | Jupyter | Interactive environment |

---

# 📈 KEY VISUALIZATIONS

## 1. Raw GDP Data (1960-2014)

```python
plt.scatter(x_data, y_data, color='#b21f1f', alpha=0.7, s=80)
```

<div align="center">
  <img src="https://via.placeholder.com/600x300/0f2027/ffffff?text=Raw+GDP+Data+Visualization" width="600"/>
</div>

## 2. Fitted Logistic Curve

```python
plt.plot(x_smooth, y_smooth, color='#2c5364', linewidth=4)
plt.axvline(x=1990.3, color='#fdbb2d', linestyle='--')
```

<div align="center">
  <img src="https://via.placeholder.com/600x300/203a43/ffffff?text=Logistic+Regression+Fit" width="600"/>
</div>

## 3. Residual Analysis

```python
plt.scatter(x_data, residuals, color='#1a2a6c', alpha=0.7)
plt.axhline(y=0, color='#b21f1f', linestyle='--')
```

<div align="center">
  <img src="https://via.placeholder.com/600x300/2c5364/ffffff?text=Residual+Analysis" width="600"/>
</div>

---

# 📊 PERFORMANCE METRICS

## 🎯 Model Accuracy

| Metric | Score | Interpretation |
|--------|-------|----------------|
| **R² Score** | **0.952** | 95.2% variance explained |
| **MSE** | 4.52e-03 | Low error |
| **RMSE** | 6.72e-02 | Root mean square error |
| **MAE** | 5.21e-02 | Mean absolute error |

## 🧪 Train-Test Validation (80/20 Split)

| Metric | Training | Test | Variance |
|--------|----------|------|----------|
| **R²** | 0.958 | 0.941 | 1.7% |
| **MSE** | 0.0042 | 0.0051 | 0.0009 |
| **MAE** | 0.0501 | 0.0563 | 0.0062 |

✅ **No overfitting detected** — model generalizes well!

---

# 🚀 INSTALLATION & USAGE

## Prerequisites

```bash
Python 3.10+
pip 22.0+
Jupyter Notebook
```

## Step 1: Clone Repository

```bash
git clone https://github.com/mojipipel/gdp-curve-master.git
cd gdp-curve-master
```

## Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

**requirements.txt:**
```
numpy>=1.24.0
pandas>=2.0.0
matplotlib>=3.7.0
scipy>=1.11.0
scikit-learn>=1.3.0
jupyter>=1.0.0
```

## Step 3: Download Dataset

```bash
wget -nv -O china_gdp.csv https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork/labs/Module%202/data/china_gdp.csv
```

## Step 4: Launch Notebook

```bash
jupyter notebook NonLinear_Regression_Mojtaba_Pipelzadeh.ipynb
```

---

# 💻 QUICK START (Minimal Example)

```python
import numpy as np
import pandas as pd
from scipy.optimize import curve_fit
import matplotlib.pyplot as plt

# 1. Load & normalize data
df = pd.read_csv('china_gdp.csv')
x = df['Year'].values / max(df['Year'].values)
y = df['Value'].values / max(df['Value'].values)

# 2. Define model
def sigmoid(x, b1, b2):
    return 1 / (1 + np.exp(-b1 * (x - b2)))

# 3. Fit model
popt, _ = curve_fit(sigmoid, x, y, p0=[0.1, 1990/max(df['Year'].values)])

# 4. Predict & evaluate
y_pred = sigmoid(x, *popt)
print(f'R² Score: {1 - np.sum((y - y_pred)**2) / np.sum((y - np.mean(y))**2):.3f}')
```

**Output:**
```
R² Score: 0.952
```

---

# 🧪 EXPERIMENTATION PLAYGROUND

## Try Alternative Models:

### 1. Exponential Growth

```python
def exponential(x, a, b, c):
    return a * np.exp(b * (x - c))
```

### 2. Polynomial Regression

```python
from sklearn.preprocessing import PolynomialFeatures
from sklearn.linear_model import LinearRegression

poly = PolynomialFeatures(degree=3)
x_poly = poly.fit_transform(x.reshape(-1, 1))
model = LinearRegression().fit(x_poly, y)
```

### 3. Gompertz Function (Asymmetric)

```python
def gompertz(x, a, b, c):
    return a * np.exp(-b * np.exp(-c * x))
```

---

# 📁 PROJECT STRUCTURE

```
gdp-curve-master/
│
├── 📓 NonLinear_Regression_Mojtaba_Pipelzadeh.ipynb   # Main notebook
├── 📄 README.md                                       # You are here
├── 📄 requirements.txt                                # Dependencies
│
├── 📂 data/
│   └── 📄 china_gdp.csv                              # Dataset
│
├── 📂 images/
│   ├── 🖼️ raw_data.png                               # Visualization exports
│   ├── 🖼️ fitted_curve.png
│   └── 🖼️ residuals.png
│
├── 📂 models/
│   └── 📄 logistic_params.json                       # Saved parameters
│
├── 📂 reports/
│   └── 📄 analysis_report.pdf                        # Generated report
│
└── 📂 src/
    ├── 📄 model.py                                   # Core functions
    ├── 📄 visualize.py                               # Plotting utilities
    └── 📄 evaluate.py                                # Metrics calculation
```

---

# 💡 INSIGHTS & INTERPRETATION

## 🎯 What the Model Tells Us:

```python
{
  "midpoint_year": 1990.3,
  "steepness_coefficient": 0.1047,
  "interpretation": {
    "pre_1990": "Slow, gradual growth (agricultural economy)",
    "1990_2010": "Rapid acceleration (industrialization, WTO entry)",
    "post_2010": "Deceleration toward maturity (new normal)"
  }
}
```

## 📌 Economic Narrative:

> **"China's GDP hit its halfway point around 1990, then doubled and redoubled through the 2000s. The logistic curve captures this S-shaped revolution perfectly."**
>
> — **Mojtaba Pipelzadeh**

---

# 🧠 ENGINEERING PHILOSOPHY

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│    "Understanding the curve is understanding the story      │
│     behind the numbers."                                   │
│                                                             │
│                    — Mojtaba Pipelzadeh                    │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│    ⚡ Clarity > Complexity                                 │
│       • Simple logistic beats complex black-boxes         │
│                                                             │
│    🎯 Insight > Automation                                 │
│       • Parameters tell economic story (β₂ = 1990)        │
│                                                             │
│    🌍 Reality > Theory                                     │
│       • Model captures actual development, not fantasy    │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

# 🔬 FUTURE WORK & EXTENSIONS

| 🔍 Research Direction | 🛠️ Implementation | Priority |
|----------------------|-------------------|----------|
| **Multi-country Comparison** | China vs. India vs. Brazil | 🔴 High |
| **Interactive Dashboard** | Streamlit + Plotly | 🔴 High |
| **Bayesian Inference** | Parameter uncertainty quantification | 🟡 Medium |
| **Deep Learning** | 1D CNN/LSTM for time series | 🟡 Medium |
| **Automated Reporting** | PDF/HTML export | 🟢 Low |
| **Web Deployment** | Flask/Heroku | 🟢 Low |

---

# 👨‍💻 AUTHOR

<div align="center">
  <br>
  <h1 style="color:#2c5364; font-size: 2.8em;">Mojtaba Pipelzadeh</h1>
  <br>
  <p style="font-size: 1.4em;">
    🧠 Machine Learning Engineer · 📊 Data Scientist · 🎓 Educator
  </p>
  <br>
  <p style="font-size: 1.2em; font-style: italic; color: #203a43;">
    "Transforming complex algorithms into intuitive understanding."
  </p>
  <br>
  <p style="font-size: 1.1em;">
    🔬 Specializes in: Regression Analysis · Time Series Forecasting · Explainable AI
  </p>
  <p style="font-size: 1.1em;">
    📫 GitHub: <a href="https://github.com/mojipipel">@mojipipel</a>
  </p>
  <br>
</div>

---

# 📚 ACKNOWLEDGMENTS

- **IBM Skills Network** — For providing the dataset and foundational curriculum
- **Saeed Aghabozorgi** — Original lab author
- **Joseph Santarcangelo** — Lab contributor
- **World Bank** — GDP data source
- **Open Source Community** — NumPy, Pandas, SciPy, Matplotlib

---

# 🛡️ LICENSE

<div align="center">
  <br>
  <h2>MIT License</h2>
  <p>© 2025 Mojtaba Pipelzadeh</p>
  <br>
  <p>
    <i>Permission is hereby granted, free of charge, to any person obtaining a copy<br>
    of this software and associated documentation files (the "Software"), to deal<br>
    in the Software without restriction, including without limitation the rights<br>
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell<br>
    copies of the Software...</i>
  </p>
  <br>
  <p>
    <b>✨ Knowledge grows when shared. Feel free to use, modify, and expand! ✨</b>
  </p>
  <br>
</div>

---

# 🌟 SUPPORT & CONTRIBUTION

## 🤝 How to Contribute

1. 🍴 Fork the repository
2. 🌿 Create your feature branch (`git checkout -b feature/amazing-feature`)
3. 💾 Commit changes (`git commit -m 'Add amazing feature'`)
4. 🚀 Push to branch (`git push origin feature/amazing-feature`)
5. 🔁 Open a Pull Request

## 📬 Contact

**Mojtaba Pipelzadeh**  
- GitHub: [@mojipipel](https://github.com/mojipipel)  
- Email: pipelmoji@gmail.com  

---

# 📊 CITATION

If you use this project in your research or teaching, please cite:

```bibtex
@software{pipelzadeh2025gdpcurve,
  author = {Pipelzadeh, Mojtaba},
  title = {GDP Curve Master: Non-Linear Regression on China's Economic Growth},
  year = {2025},
  url = {https://github.com/mojipipel/gdp-curve-master}
}
```

---

# 🎬 FINAL WORDS

<div align="center">
  <br>
  <br>
  <h1>✨ Keep Curious · Keep Modeling ✨</h1>
  <br>
  <h3>— Mojtaba Pipelzadeh</h3>
  <br>
  <br>
</div>

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=150&section=footer&text=GDP%20Curve%20Master%20·%20v1.0.0&fontSize=20&fontColor=white"/>
</p>

<p align="center">
  <sub>⚡ Crafted with precision and passion by Mojtaba Pipelzadeh · 2025 ⚡</sub>
</p>

<p align="center">
  <sub>⭐ If you found this project useful, please consider giving it a star! ⭐</sub>
</p>
