<div align="center">

# 🌈📊 **SEABORN TIPS DATA ANALYSIS REPORT**
### ✨ *Exploratory Data Analysis using Pandas, NumPy, Matplotlib & Seaborn* ✨

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=28&pause=1000&color=FF0000&center=true&vCenter=true&width=900&lines=Data+Analysis+Project;Seaborn+Tips+Dataset+Exploration;Pandas+%7C+NumPy+%7C+Matplotlib+%7C+Seaborn;Visualizing+Customer+Tipping+Behavior" />

---

![Dashboard](dashboard-overview.png)

</div>

---

# 🎯 Introduction & Objective

> The **Tips Dataset** is one of the most popular sample datasets available in Seaborn. It contains information collected from restaurant bills and tips, making it ideal for practicing **Exploratory Data Analysis (EDA)**, statistical summaries, and visualization techniques.

## 📌 Project Objectives

- Understand the structure of the dataset.
- Explore relationships between restaurant bills and tips.
- Analyze customer behavior based on:
  - Gender
  - Smoking status
  - Day of the week
  - Time of dining
  - Party size
- Identify patterns, trends, and anomalies.
- Create meaningful visualizations using Seaborn and Matplotlib.
- Generate actionable insights from the data.

---

# 📚 Libraries Used

| Library | Purpose |
|----------|----------|
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical graphics and advanced visualizations |

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

# 📂 Dataset Overview

The dataset contains information about restaurant customers and the tips they left.

## Dataset Information

| Column | Description |
|----------|-------------|
| total_bill | Total restaurant bill amount |
| tip | Tip given by customer |
| sex | Gender of customer |
| smoker | Whether customer is smoker |
| day | Day of visit |
| time | Lunch or Dinner |
| size | Number of people in group |

---

## Dataset Shape

```python
tips.shape
```

Expected Output:

```python
(244, 7)
```

---

## Column Information

```python
tips.columns
```

Output:

```python
Index([
'total_bill',
'tip',
'sex',
'smoker',
'day',
'time',
'size'
])
```

---

## Data Types

```python
tips.dtypes
```

| Column | Data Type |
|----------|------------|
| total_bill | float64 |
| tip | float64 |
| sex | category/object |
| smoker | category/object |
| day | category/object |
| time | category/object |
| size | int64 |

---

## Missing Values Check

```python
tips.isnull().sum()
```

Expected Output:

```python
total_bill    0
tip           0
sex           0
smoker        0
day           0
time          0
size          0
```

✅ No missing values found.

---

# 🚀 Data Loading & Initial Exploration

## Load Dataset

```python
tips = sns.load_dataset("tips")
tips.head()
```

---

## First Five Records

| total_bill | tip | sex | smoker | day | time | size |
|------------|-----|------|------|------|------|------|
| 16.99 | 1.01 | Female | No | Sun | Dinner | 2 |
| 10.34 | 1.66 | Male | No | Sun | Dinner | 3 |
| 21.01 | 3.50 | Male | No | Sun | Dinner | 3 |

---

## Basic Dataset Information

```python
tips.info()
```

---

## Statistical Summary

```python
tips.describe()
```

Provides:

- Count
- Mean
- Standard Deviation
- Minimum
- Quartiles
- Maximum

---

# 🧹 Data Cleaning & Preprocessing

Even though the Tips dataset is clean, the following best practices should always be applied.

---

## Missing Values Handling

```python
tips.isnull().sum()
```

If present:

```python
tips.fillna(tips.mean(numeric_only=True))
```

---

## Duplicate Records

```python
tips.duplicated().sum()
```

Remove duplicates:

```python
tips = tips.drop_duplicates()
```

---

## Outlier Detection

### Using IQR Method

```python
Q1 = tips['total_bill'].quantile(0.25)
Q3 = tips['total_bill'].quantile(0.75)

IQR = Q3 - Q1

lower = Q1 - 1.5 * IQR
upper = Q3 + 1.5 * IQR

outliers = tips[
    (tips['total_bill'] < lower) |
    (tips['total_bill'] > upper)
]
```

---

## Feature Engineering

### Tip Percentage

```python
tips["tip_percent"] = (
    tips["tip"] /
    tips["total_bill"]
) * 100
```

Example:

| total_bill | tip | tip_percent |
|------------|------|------------|
| 20 | 4 | 20% |

---

# 🔍 Exploratory Data Analysis (EDA)

---

# 📈 Univariate Analysis

Univariate analysis focuses on understanding individual variables.

---

## Distribution of Total Bill

```python
plt.figure(figsize=(8,5))

sns.histplot(
    tips["total_bill"],
    kde=True,
    bins=20
)

plt.title("Distribution of Total Bill")
plt.show()
```

![Total Bill Distribution](total-bill-distribution.png)

### Insights

- Right-skewed distribution
- Majority of bills between \$10-\$25
- Few high-value bills

---

## Distribution of Tips

```python
sns.histplot(
    tips["tip"],
    kde=True
)
```

![Tip Distribution](tip-distribution.png)

### Findings

- Most tips range from \$2-\$4
- Positive skew observed

---

## Boxplot Analysis

```python
sns.boxplot(
    y=tips["total_bill"]
)
```

![Boxplot Total Bill](boxplot-totalbill.png)

### Purpose

- Detect outliers
- Visualize spread
- Understand quartiles

---

## Count Plot of Days

```python
sns.countplot(
    data=tips,
    x="day"
)
```

![Day Count Plot](day-countplot.png)

### Observation

Weekend traffic dominates restaurant visits.

---

# 📊 Bivariate Analysis

Bivariate analysis studies relationships between two variables.

---

## Total Bill vs Tip

```python
plt.figure(figsize=(8,5))

sns.scatterplot(
    data=tips,
    x="total_bill",
    y="tip",
    hue="sex"
)
```

![Scatter Plot](scatter-totalbill-tip.png)

### Insights

- Positive correlation observed
- Higher bills generally generate larger tips

---

## Average Tips by Gender

```python
sns.barplot(
    data=tips,
    x="sex",
    y="tip"
)
```

![Gender Tip Analysis](gender-tip-analysis.png)

---

## Tips by Smoking Status

```python
sns.boxplot(
    data=tips,
    x="smoker",
    y="tip"
)
```

![Smoker Analysis](smoker-tip-analysis.png)

---

## Time vs Total Bill

```python
sns.violinplot(
    data=tips,
    x="time",
    y="total_bill"
)
```

![Time Analysis](time-analysis.png)

### Findings

- Dinner bills tend to be larger
- Greater variation during dinner

---

# 🌐 Multivariate Analysis

Multivariate analysis evaluates relationships among multiple variables simultaneously.

---

## Pairplot

```python
sns.pairplot(
    tips,
    hue="sex"
)
```

![Pairplot](pairplot-analysis.png)

### Benefits

- Relationship discovery
- Distribution overview
- Cluster identification

---

## Correlation Heatmap

```python
corr = tips.corr(
    numeric_only=True
)

plt.figure(figsize=(8,6))

sns.heatmap(
    corr,
    annot=True,
    cmap="rainbow"
)

plt.show()
```

![Correlation Heatmap](correlation-heatmap.png)

---

## Interpretation

| Variable Pair | Correlation |
|--------------|------------|
| total_bill ↔ tip | Strong Positive |
| size ↔ total_bill | Moderate Positive |
| size ↔ tip | Moderate Positive |

---

## Average Bill by Day & Time

```python
pivot = tips.pivot_table(
    values="total_bill",
    index="day",
    columns="time",
    aggfunc="mean"
)

sns.heatmap(
    pivot,
    annot=True,
    cmap="Spectral"
)
```

![Day Time Heatmap](day-time-heatmap.png)

---

# 📊 Statistical Summary

## Numerical Features

```python
tips.describe()
```

| Metric | Total Bill | Tip | Size |
|---------|------------|------|------|
| Mean | 19.79 | 2.99 | 2.57 |
| Median | 17.80 | 2.90 | 2 |
| Std Dev | 8.90 | 1.38 | 0.95 |
| Min | 3.07 | 1.00 | 1 |
| Max | 50.81 | 10.00 | 6 |

---

## Grouped Statistics

### Average Tip by Day

```python
tips.groupby("day")["tip"].mean()
```

### Average Bill by Time

```python
tips.groupby("time")["total_bill"].mean()
```

---

# 💡 Key Insights & Findings

## 🔥 Major Discoveries

### 💰 Billing Trends

- Higher bills generally lead to larger tips.
- Most customer bills are between **\$10 and \$25**.
- Large bills are relatively rare.

### 🍽 Dining Behavior

- Dinner generates larger bills than lunch.
- Weekend visits dominate restaurant traffic.

### 👥 Group Size Impact

- Larger groups tend to spend more.
- Larger groups usually leave higher tips.

### 🚬 Smoking Analysis

- Smoking status shows slight differences in tipping patterns.
- Distribution overlap suggests limited impact.

### 📊 Correlation Findings

- Strong positive relationship between:
  - Total Bill ↔ Tip
- Moderate positive relationship between:
  - Group Size ↔ Bill
  - Group Size ↔ Tip

---

# 🎨 Visualizations Gallery

---

## 1️⃣ Distribution of Total Bill

![Distribution Plot](distribution-totalbill.png)

Purpose:

- Understand spending patterns
- Detect skewness

---

## 2️⃣ Distribution of Tips

![Tips Histogram](tips-histogram.png)

Purpose:

- Analyze tipping behavior

---

## 3️⃣ Total Bill Boxplot

![Total Bill Boxplot](totalbill-boxplot.png)

Purpose:

- Detect outliers

---

## 4️⃣ Tip Boxplot

![Tip Boxplot](tip-boxplot.png)

Purpose:

- Visualize variability

---

## 5️⃣ Scatter Plot

![Scatter Plot](bill-tip-scatter.png)

Purpose:

- Relationship between bill and tip

---

## 6️⃣ Gender Comparison

![Gender Comparison](gender-comparison.png)

Purpose:

- Compare tipping patterns

---

## 7️⃣ Smoking Analysis

![Smoking Analysis](smoking-analysis.png)

Purpose:

- Explore smoker vs non-smoker behavior

---

## 8️⃣ Pairplot

![Pairplot](pairplot.png)

Purpose:

- Comprehensive feature interaction analysis

---

## 9️⃣ Correlation Heatmap

![Heatmap](heatmap.png)

Purpose:

- Visualize feature relationships

---

## 🔟 Day-Time Spending Heatmap

![Day Time Heatmap](daytime-heatmap.png)

Purpose:

- Compare average spending patterns

---

# 🏆 Best Practices Used

## Pandas

✅ Use `.info()` before analysis

✅ Check missing values

```python
df.isnull().sum()
```

✅ Use grouping effectively

```python
df.groupby("category").mean()
```

---

## NumPy

✅ Vectorized calculations

```python
df["tip_percent"] = (
    df["tip"] /
    df["total_bill"]
) * 100
```

---

## Matplotlib

✅ Always define figure size

```python
plt.figure(figsize=(10,6))
```

✅ Add titles and labels

```python
plt.title("Plot Title")
plt.xlabel("X Label")
plt.ylabel("Y Label")
```

---

## Seaborn

✅ Use themes

```python
sns.set_theme(
    style="whitegrid"
)
```

✅ Use color palettes

```python
sns.set_palette(
    "rainbow"
)
```

✅ Add annotations where useful

```python
sns.heatmap(
    corr,
    annot=True
)
```

---

# 🎯 Conclusion & Recommendations

The **Tips Dataset Analysis** successfully revealed customer spending and tipping patterns through descriptive statistics and visualization techniques.

### Key Conclusions

✔ Strong positive relationship exists between bill amount and tip.

✔ Dinner customers spend more than lunch customers.

✔ Larger groups contribute to higher restaurant revenue.

✔ Weekend activity dominates overall restaurant business.

✔ Data quality is excellent with no missing values.

### Recommendations

📌 Focus promotional campaigns during weekends.

📌 Encourage larger group reservations.

📌 Monitor high-value customers for loyalty programs.

📌 Utilize predictive models to estimate expected tips and revenue.

---

# 🚀 Future Scope

The analysis can be extended further using advanced techniques:

### 🤖 Machine Learning

- Tip Prediction Model
- Revenue Forecasting
- Customer Segmentation

### 📈 Advanced Analytics

- Hypothesis Testing
- Confidence Intervals
- ANOVA
- Regression Analysis

### 📊 Interactive Dashboards

- Plotly Dash
- Streamlit
- Power BI
- Tableau

### ☁ Big Data Expansion

- Real-time restaurant analytics
- Customer behavior monitoring
- Dynamic pricing analysis

---

<div align="center">

# 🌈 Thank You

### 📊 *Data Analysis using Pandas • NumPy • Matplotlib • Seaborn*

✨ Turning restaurant data into actionable insights through visualization and analytics ✨

</div>
