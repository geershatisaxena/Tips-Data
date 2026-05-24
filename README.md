<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF0080,25:FF6B35,50:FFD700,75:00FF88,100:00BFFF&height=220&section=header&text=SEABORN%20TIPS%20DATA%20ANALYSIS&fontSize=38&fontColor=ffffff&fontAlignY=38&desc=Exploratory%20Data%20Analysis%20%7C%20Pandas%20%E2%80%A2%20NumPy%20%E2%80%A2%20Matplotlib%20%E2%80%A2%20Seaborn&descAlignY=58&descSize=16&animation=twinkling" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=900&size=26&pause=1200&color=FF0080&center=true&vCenter=true&width=900&lines=%F0%9F%8C%88+Welcome+to+the+Ultimate+EDA+Report!;%F0%9F%94%AC+Uncovering+Patterns+in+Restaurant+Tips;%F0%9F%93%8A+Visualizing+Customer+Tipping+Behavior;%F0%9F%A4%96+Powered+by+Pandas+%7C+NumPy+%7C+Seaborn;%F0%9F%9A%80+Data+Science+%7C+Insights+%7C+Analytics" alt="Typing SVG" />

<br/><br/>

<img src="https://img.shields.io/badge/Python-3.10+-FF0080?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Pandas-2.0-FF6B35?style=for-the-badge&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/NumPy-1.25-FFD700?style=for-the-badge&logo=numpy&logoColor=white" />
<img src="https://img.shields.io/badge/Seaborn-0.13-00FF88?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Matplotlib-3.8-00BFFF?style=for-the-badge&logo=python&logoColor=white" />

<br/><br/>

<img src="https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge" />
<img src="https://img.shields.io/badge/Dataset-244%20Records-purple?style=for-the-badge" />
<img src="https://img.shields.io/badge/Features-7%20Columns-FF6B35?style=for-the-badge" />
<img src="https://img.shields.io/badge/Missing%20Values-None-00FF88?style=for-the-badge" />

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:FF0080,50:8B00FF,100:00BFFF&height=3&section=header" />
</div>

---

<h2><img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=700&size=20&pause=2000&color=FF6B35&center=false&vCenter=true&width=600&lines=%F0%9F%8E%AF+Introduction+%26+Project+Objectives" /></h2>

<table>
<tr>
<td width="65%">

> 🍽️ The **Tips Dataset** is a classic sample dataset available in the Seaborn library. It captures real-world restaurant billing and tipping data — perfect for practicing **Exploratory Data Analysis (EDA)**, statistical summaries, and producing publication-quality visualizations.
>
> This report takes a deep-dive analytical approach to uncover hidden patterns, behavioral trends, and actionable business insights from the dataset — all presented with vibrant, production-grade visualizations.

</td>
<td width="35%" align="center">

```
📦 Dataset Facts
━━━━━━━━━━━━━━━
📋 244 records
🏷️  7 features
🎯  0 nulls
📅  4 days tracked
🍽️  2 meal times
👥  Party size 1–6
💰  Bills $3–$51
```

</td>
</tr>
</table>

### 🌈 Project Objectives

<table>
<tr>
<td>🔵 <b>Understand</b> the dataset structure and variable types</td>
<td>🟣 <b>Explore</b> bill-to-tip relationships</td>
</tr>
<tr>
<td>🟠 <b>Analyze</b> behavior by gender, smoking, day & time</td>
<td>🟡 <b>Detect</b> outliers and distribution shapes</td>
</tr>
<tr>
<td>🟢 <b>Engineer</b> new features for richer analysis</td>
<td>🔴 <b>Visualize</b> patterns with Seaborn & Matplotlib</td>
</tr>
<tr>
<td>🩵 <b>Correlate</b> numerical variables via heatmaps</td>
<td>💜 <b>Derive</b> actionable business insights</td>
</tr>
</table>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:FF0080,25:FF6B35,50:FFD700,75:00FF88,100:00BFFF&height=4" />
</div>

<h2>📚 <span style="background: linear-gradient(90deg, #FF0080, #FF6B35, #FFD700); -webkit-background-clip: text;">Libraries & Technology Stack</span></h2>

<div align="center">

| 🔧 Library | 🎨 Version | 🚀 Primary Role | 🌈 Use Case |
|:----------:|:-----------:|:----------------:|:-----------:|
| ![Pandas](https://img.shields.io/badge/Pandas-FF0080?style=flat-square&logo=pandas&logoColor=white) | `2.0+` | Data Manipulation | Loading, filtering, grouping, aggregating |
| ![NumPy](https://img.shields.io/badge/NumPy-FF6B35?style=flat-square&logo=numpy&logoColor=white) | `1.25+` | Numerical Computing | Vectorized ops, IQR, statistics |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-FFD700?style=flat-square&logo=python&logoColor=black) | `3.8+` | Base Visualization | Figure setup, axis control, subplots |
| ![Seaborn](https://img.shields.io/badge/Seaborn-00FF88?style=flat-square&logo=python&logoColor=black) | `0.13+` | Statistical Plots | Histograms, boxplots, heatmaps, pairplots |

</div>

```python
# 🌈 Import All Required Libraries
import pandas as pd           # 🔴 Data manipulation
import numpy as np            # 🟠 Numerical computing
import matplotlib.pyplot as plt  # 🟡 Base plotting
import seaborn as sns         # 🟢 Statistical visualization
import warnings

# 🎨 Configure Style
sns.set_theme(style="whitegrid", palette="husl")
plt.rcParams["figure.dpi"] = 150
warnings.filterwarnings("ignore")

print("✅ All libraries loaded successfully!")
```

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:8B00FF,50:FF0080,100:FF6B35&height=4" />
</div>

<h2>📂 <span style="color:#FF0080">Dataset Overview</span></h2>

### 🗂️ Column Descriptions

<div align="center">

| # | 🏷️ Column | 📊 Data Type | 📝 Description | 🌈 Category |
|:-:|:---------:|:------------:|:--------------:|:-----------:|
| 1 | `total_bill` | `float64` | Total restaurant bill in USD | 💰 Numerical |
| 2 | `tip` | `float64` | Tip amount given by customer | 💵 Numerical |
| 3 | `sex` | `category` | Gender of the bill-paying customer | 👤 Categorical |
| 4 | `smoker` | `category` | Whether the customer smokes | 🚬 Categorical |
| 5 | `day` | `category` | Day of the week (Thu–Sun) | 📅 Categorical |
| 6 | `time` | `category` | Meal time — Lunch or Dinner | 🍽️ Categorical |
| 7 | `size` | `int64` | Number of people in the party | 👥 Numerical |

</div>

### 📊 Statistical Summary Cards

<div align="center">

| 📈 Metric | 💰 Total Bill | 💵 Tip | 👥 Party Size |
|:---------:|:------------:|:------:|:-------------:|
| 🔢 **Count** | 244 | 244 | 244 |
| 📊 **Mean** | $19.79 | $2.99 | 2.57 |
| 📉 **Median** | $17.80 | $2.90 | 2 |
| 📐 **Std Dev** | $8.90 | $1.38 | 0.95 |
| ⬇️ **Min** | $3.07 | $1.00 | 1 |
| 📌 **Q1 (25%)** | $13.35 | $2.00 | 2 |
| 📌 **Q3 (75%)** | $24.13 | $3.56 | 3 |
| ⬆️ **Max** | $50.81 | $10.00 | 6 |

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:FFD700,50:00FF88,100:00BFFF&height=4" />
</div>

<h2>🚀 <span style="color:#00FF88">Data Loading & Initial Exploration</span></h2>

### 📥 Load the Dataset

```python
# 🌈 Load Seaborn Tips Dataset
tips = sns.load_dataset("tips")

# 🔍 Preview first 5 rows
print("📋 First 5 Records:")
print(tips.head())
```

### 👀 First Five Records

<div align="center">

| total_bill | tip | sex | smoker | day | time | size |
|:----------:|:---:|:---:|:------:|:---:|:----:|:----:|
| 16.99 | 1.01 | Female | No | Sun | Dinner | 2 |
| 10.34 | 1.66 | Male | No | Sun | Dinner | 3 |
| 21.01 | 3.50 | Male | No | Sun | Dinner | 3 |
| 23.68 | 3.31 | Male | No | Sun | Dinner | 2 |
| 24.59 | 3.61 | Female | No | Sun | Dinner | 4 |

</div>

### 📐 Dataset Shape & Info

```python
# 📦 Dataset dimensions
print(f"🔢 Shape: {tips.shape}")        # (244, 7)
print(f"📋 Columns: {list(tips.columns)}")

# 🔎 Detailed info
tips.info()

# 📊 Statistical summary
tips.describe()
```

```
📦 Shape: (244, 7)
📋 Columns: ['total_bill', 'tip', 'sex', 'smoker', 'day', 'time', 'size']

RangeIndex: 244 entries, 0 to 243
Data columns (total 7 columns):
 #   Column      Non-Null Count  Dtype
---  ------      --------------  -----
 0   total_bill  244 non-null    float64
 1   tip         244 non-null    float64
 2   sex         244 non-null    category
 3   smoker      244 non-null    category
 4   day         244 non-null    category
 5   time        244 non-null    category
 6   size        244 non-null    int64
```

### 🔢 Categorical Value Counts

```python
# 🌈 Explore categorical distributions
for col in ['sex', 'smoker', 'day', 'time']:
    print(f"\n📊 {col.upper()} Distribution:")
    print(tips[col].value_counts())
```

```
📊 SEX Distribution:           📊 SMOKER Distribution:
Male      157                  No     151
Female     87                  Yes     93

📊 DAY Distribution:           📊 TIME Distribution:
Sat    87                      Dinner    176
Sun    76                      Lunch      68
Thur   62
Fri    19
```

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00BFFF,50:8B00FF,100:FF0080&height=4" />
</div>

<h2>🧹 <span style="color:#00BFFF">Data Cleaning & Preprocessing</span></h2>

### ✅ Missing Values Audit

```python
# 🔍 Check for any missing values
missing = tips.isnull().sum()
print("🔎 Missing Values per Column:")
print(missing)

# Output:
# total_bill    0  ✅
# tip           0  ✅
# sex           0  ✅
# smoker        0  ✅
# day           0  ✅
# time          0  ✅
# size          0  ✅
```

> 🎉 **Result:** Zero missing values across all 7 columns — dataset is pristine!

### 🔁 Duplicate Records Check

```python
# 🔁 Identify duplicates
duplicates = tips.duplicated().sum()
print(f"⚠️  Duplicate Rows Found: {duplicates}")

# Remove if any exist
tips = tips.drop_duplicates()
print(f"✅ Clean Dataset Shape: {tips.shape}")
```

### 📦 Outlier Detection — IQR Method

```python
# 📦 IQR-based outlier detection for total_bill
Q1 = tips['total_bill'].quantile(0.25)   # 13.35
Q3 = tips['total_bill'].quantile(0.75)   # 24.13
IQR = Q3 - Q1                            # 10.78

lower_bound = Q1 - 1.5 * IQR            # ~-2.82 (floor = 0)
upper_bound = Q3 + 1.5 * IQR            # ~40.30

outliers = tips[
    (tips['total_bill'] < lower_bound) |
    (tips['total_bill'] > upper_bound)
]

print(f"🚨 Outliers Detected: {len(outliers)} records")
print(outliers[['total_bill', 'tip', 'size']])
```

### ⚗️ Feature Engineering

```python
# 💡 Create new derived feature: Tip Percentage
tips["tip_percent"] = (tips["tip"] / tips["total_bill"]) * 100

# 💡 Tip per person
tips["tip_per_person"] = tips["tip"] / tips["size"]

# 💡 Bill per person
tips["bill_per_person"] = tips["total_bill"] / tips["size"]

print("✅ New Features Created:")
print(tips[["total_bill", "tip", "tip_percent",
            "tip_per_person", "bill_per_person"]].head())
```

<div align="center">

| total_bill | tip | tip_percent | tip_per_person | bill_per_person |
|:----------:|:---:|:-----------:|:--------------:|:---------------:|
| 16.99 | 1.01 | 5.94% | 0.505 | 8.495 |
| 10.34 | 1.66 | 16.05% | 0.553 | 3.447 |
| 21.01 | 3.50 | 16.66% | 1.167 | 7.003 |
| 23.68 | 3.31 | 13.98% | 1.655 | 11.84 |
| 24.59 | 3.61 | 14.68% | 0.903 | 6.148 |

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:FF0080,20:FF6B35,40:FFD700,60:00FF88,80:00BFFF,100:8B00FF&height=5" />
</div>

<h2>🔍 <span style="color:#FFD700">Exploratory Data Analysis (EDA)</span></h2>

<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=700&size=16&pause=2000&color=FFD700&center=false&vCenter=true&width=700&lines=%F0%9F%93%8A+Diving+Deep+into+Patterns+%26+Distributions..." />

---

### 📈 1. Univariate Analysis

#### 📊 Distribution of Total Bill

```python
fig, axes = plt.subplots(1, 2, figsize=(14, 5))

# 🌈 Histogram with KDE
sns.histplot(
    tips["total_bill"],
    kde=True,
    bins=25,
    color="#FF0080",
    ax=axes[0]
)
axes[0].set_title("🧾 Distribution of Total Bill", fontsize=14, fontweight='bold')
axes[0].set_xlabel("Total Bill ($)")
axes[0].set_ylabel("Frequency")

# 📦 Boxplot
sns.boxplot(
    y=tips["total_bill"],
    color="#FF6B35",
    ax=axes[1]
)
axes[1].set_title("📦 Boxplot — Total Bill", fontsize=14, fontweight='bold')

plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Distribution of Total Bill — Rainbow Theme](plot_01_total_bill_distribution.png)

> 🔎 **Insights:** Right-skewed distribution. Most bills fall between **$10–$25**. A few high-value outliers exist above $40.

---

#### 💵 Distribution of Tips

```python
fig, axes = plt.subplots(1, 2, figsize=(14, 5))

sns.histplot(
    tips["tip"],
    kde=True,
    bins=20,
    color="#8B00FF",
    ax=axes[0]
)
axes[0].set_title("💵 Distribution of Tips", fontsize=14, fontweight='bold')

sns.boxplot(
    y=tips["tip"],
    color="#00BFFF",
    ax=axes[1]
)
axes[1].set_title("📦 Boxplot — Tips", fontsize=14, fontweight='bold')

plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Distribution of Tips — Rainbow Theme](plot_02_tip_distribution.png)

> 🔎 **Insights:** Tips are mostly between **$2–$4**. Positive skew with peak around $2. Occasional generous tippers push the max to $10.

---

#### 📅 Count of Visits by Day

```python
plt.figure(figsize=(8, 5))

palette = ["#FF0080", "#FF6B35", "#FFD700", "#00FF88"]

sns.countplot(
    data=tips,
    x="day",
    palette=palette,
    order=["Thur", "Fri", "Sat", "Sun"]
)

plt.title("📅 Restaurant Visits by Day of Week",
          fontsize=14, fontweight='bold')
plt.xlabel("Day")
plt.ylabel("Number of Visits")
plt.show()
```

> 📌 **Plot Placeholder**

![Count Plot — Visits by Day of Week](plot_03_day_countplot.png)

> 🔎 **Insights:** **Saturday** sees the most traffic (87 visits), followed by Sunday. Weekends dominate restaurant business significantly.

---

#### 🚬 Smoker vs Non-Smoker Count

```python
sns.countplot(
    data=tips,
    x="smoker",
    palette=["#00FF88", "#FF0080"]
)
plt.title("🚬 Smoker vs Non-Smoker Count")
plt.show()
```

> 📌 **Plot Placeholder**

![Smoker Count Plot](plot_04_smoker_count.png)

---

### 📊 2. Bivariate Analysis

#### 💡 Total Bill vs Tip (Scatter Plot)

```python
plt.figure(figsize=(10, 6))

sns.scatterplot(
    data=tips,
    x="total_bill",
    y="tip",
    hue="sex",
    style="time",
    size="size",
    sizes=(50, 300),
    palette=["#FF0080", "#00BFFF"],
    alpha=0.8
)

plt.title("💡 Total Bill vs Tip — Colored by Gender",
          fontsize=14, fontweight='bold')
plt.xlabel("Total Bill ($)")
plt.ylabel("Tip ($)")
plt.legend(bbox_to_anchor=(1.05, 1))
plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Scatter Plot — Total Bill vs Tip with Gender & Time](plot_05_scatter_bill_tip.png)

> 🔎 **Insights:** Clear **positive correlation** between total bill and tip amount. Both genders follow a similar trend. Larger parties (bigger bubbles) tend to have higher bills.

---

#### 👥 Average Tip by Gender

```python
fig, axes = plt.subplots(1, 2, figsize=(12, 5))

# Bar plot
sns.barplot(
    data=tips,
    x="sex",
    y="tip",
    palette=["#FF0080", "#00BFFF"],
    ax=axes[0],
    capsize=0.1
)
axes[0].set_title("👥 Average Tip by Gender")

# Violin plot
sns.violinplot(
    data=tips,
    x="sex",
    y="tip",
    palette=["#FF6B35", "#8B00FF"],
    ax=axes[1],
    inner="box"
)
axes[1].set_title("🎻 Tip Distribution by Gender")

plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Gender Tip Analysis — Bar & Violin](plot_06_gender_tip_analysis.png)

> 🔎 **Insights:** Males tip slightly more on average ($3.09) vs Females ($2.83), but the difference is modest. Distribution shapes are similar.

---

#### 🍽️ Tips by Meal Time

```python
fig, axes = plt.subplots(1, 2, figsize=(12, 5))

sns.boxplot(
    data=tips,
    x="time",
    y="total_bill",
    palette=["#FFD700", "#FF0080"],
    ax=axes[0]
)
axes[0].set_title("🍽️ Bill by Meal Time")

sns.violinplot(
    data=tips,
    x="time",
    y="tip",
    palette=["#00FF88", "#8B00FF"],
    ax=axes[1],
    inner="quartile"
)
axes[1].set_title("🎻 Tip Distribution by Time")

plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Meal Time Analysis — Box & Violin](plot_07_time_analysis.png)

> 🔎 **Insights:** **Dinner** shows both higher bills and greater spending variability compared to Lunch. Dinner median bill is ~$20 vs ~$15 for Lunch.

---

#### 📅 Tips by Day of Week

```python
plt.figure(figsize=(10, 5))

sns.boxplot(
    data=tips,
    x="day",
    y="tip",
    palette=["#FF0080", "#FF6B35", "#FFD700", "#00FF88"],
    order=["Thur", "Fri", "Sat", "Sun"]
)

plt.title("📅 Tip Distribution by Day of Week",
          fontsize=14, fontweight='bold')
plt.xlabel("Day")
plt.ylabel("Tip ($)")
plt.show()
```

> 📌 **Plot Placeholder**

![Tip Box Plot by Day of Week](plot_08_tips_by_day.png)

---

#### 🚬 Smoking Status & Tipping

```python
fig, axes = plt.subplots(1, 2, figsize=(12, 5))

sns.boxplot(
    data=tips,
    x="smoker",
    y="tip",
    palette=["#00BFFF", "#FF6B35"],
    ax=axes[0]
)
axes[0].set_title("🚬 Tips: Smoker vs Non-Smoker (Box)")

sns.stripplot(
    data=tips,
    x="smoker",
    y="tip",
    palette=["#8B00FF", "#FFD700"],
    jitter=True,
    alpha=0.6,
    ax=axes[1]
)
axes[1].set_title("📍 Tips: Smoker vs Non-Smoker (Strip)")

plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Smoker Tip Analysis](plot_09_smoker_tip_analysis.png)

---

### 🌐 3. Multivariate Analysis

#### 🔗 Comprehensive Pairplot

```python
# 🌈 Pairplot with gender hue
pair_vars = ["total_bill", "tip", "size", "tip_percent"]

g = sns.pairplot(
    tips[pair_vars + ["sex"]],
    hue="sex",
    palette=["#FF0080", "#00BFFF"],
    diag_kind="kde",
    plot_kws={"alpha": 0.6, "s": 40},
    diag_kws={"shade": True}
)

g.fig.suptitle("🔗 Pairplot — Tips Dataset (Hue: Gender)",
               y=1.02, fontsize=16, fontweight='bold')
plt.show()
```

> 📌 **Plot Placeholder**

![Comprehensive Pairplot — Gender Hue](plot_10_pairplot.png)

---

#### 🌡️ Correlation Heatmap

```python
# 🌡️ Compute correlation matrix
corr_matrix = tips[
    ["total_bill", "tip", "size", "tip_percent", "tip_per_person"]
].corr()

plt.figure(figsize=(9, 7))

mask = np.triu(np.ones_like(corr_matrix, dtype=bool))

sns.heatmap(
    corr_matrix,
    annot=True,
    fmt=".2f",
    cmap="coolwarm",
    mask=mask,
    linewidths=2,
    linecolor='white',
    square=True,
    cbar_kws={"shrink": 0.8},
    annot_kws={"size": 12, "weight": "bold"}
)

plt.title("🌡️ Correlation Heatmap — Numerical Features",
          fontsize=14, fontweight='bold', pad=20)
plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Correlation Heatmap — Rainbow Coolwarm Theme](plot_11_correlation_heatmap.png)

#### 📐 Correlation Interpretation

<div align="center">

| 🔗 Variable Pair | 📊 Correlation | 🎨 Strength | 📝 Interpretation |
|:----------------:|:--------------:|:-----------:|:------------------:|
| `total_bill` ↔ `tip` | **+0.68** | 🔴 Strong Positive | Higher bills → larger tips |
| `size` ↔ `total_bill` | **+0.60** | 🟠 Moderate Positive | Bigger parties → higher bills |
| `size` ↔ `tip` | **+0.49** | 🟡 Moderate Positive | Bigger parties → more tip |
| `tip_percent` ↔ `total_bill` | **−0.11** | 🟢 Weak Negative | Big spenders tip slightly less % |
| `size` ↔ `tip_percent` | **−0.03** | 🔵 Negligible | Party size barely affects % tip |

</div>

---

#### 🗓️ Day × Time Pivot Heatmap

```python
# 📊 Average bill by day and time
pivot_bill = tips.pivot_table(
    values="total_bill",
    index="day",
    columns="time",
    aggfunc="mean"
)

pivot_tip = tips.pivot_table(
    values="tip",
    index="day",
    columns="time",
    aggfunc="mean"
)

fig, axes = plt.subplots(1, 2, figsize=(14, 5))

sns.heatmap(
    pivot_bill,
    annot=True,
    fmt=".1f",
    cmap="YlOrRd",
    ax=axes[0],
    linewidths=2,
    cbar_kws={"label": "Avg Bill ($)"}
)
axes[0].set_title("💰 Avg Total Bill by Day & Time")

sns.heatmap(
    pivot_tip,
    annot=True,
    fmt=".2f",
    cmap="PuBuGn",
    ax=axes[1],
    linewidths=2,
    cbar_kws={"label": "Avg Tip ($)"}
)
axes[1].set_title("💵 Avg Tip by Day & Time")

plt.tight_layout()
plt.show()
```

> 📌 **Plot Placeholder**

![Day-Time Pivot Heatmap](plot_12_day_time_heatmap.png)

---

#### 🎭 FacetGrid — Bills by Smoker & Gender

```python
g = sns.FacetGrid(
    tips,
    col="smoker",
    row="sex",
    height=4,
    aspect=1.2,
    palette="husl"
)

g.map_dataframe(
    sns.scatterplot,
    x="total_bill",
    y="tip",
    hue="time",
    palette=["#FF0080", "#00BFFF"],
    alpha=0.7
)

g.add_legend()
g.set_titles(col_template="🚬 Smoker: {col_name}",
             row_template="👤 {row_name}")
g.fig.suptitle("🎭 FacetGrid — Bill vs Tip by Gender & Smoking",
               y=1.02, fontsize=14, fontweight='bold')
plt.show()
```

> 📌 **Plot Placeholder**

![FacetGrid — Smoker × Gender Analysis](plot_13_facetgrid.png)

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00FF88,33:00BFFF,66:8B00FF,100:FF0080&height=4" />
</div>

<h2>💡 <span style="color:#00FF88">Key Insights & Findings</span></h2>

<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=600&size=15&pause=2000&color=00FF88&center=false&vCenter=true&width=700&lines=%F0%9F%94%AC+Here's+What+the+Data+Revealed..." />

---

<table>
<tr>
<td width="50%">

### 💰 Billing Trends
> 🔴 Most bills fall in the **$10–$25** range<br/>
> 🟠 Average bill: **$19.79**<br/>
> 🟡 High-value bills (>$40) are rare outliers<br/>
> 🟢 Bill distribution is **right-skewed**

</td>
<td width="50%">

### 🍽️ Dining Behavior
> 🔵 **Dinner** consistently generates higher bills<br/>
> 💜 **Saturdays** are the busiest day (87 visits)<br/>
> 🩵 Weekends account for ~67% of all visits<br/>
> 🌸 Friday is the quietest day (19 visits)

</td>
</tr>
<tr>
<td>

### 👥 Group Size Impact
> 🔴 Larger groups spend **significantly more**<br/>
> 🟠 Group size & bill: **+0.60 correlation**<br/>
> 🟡 Groups of 5–6 drive the largest bills<br/>
> 🟢 Median party size is just **2 people**

</td>
<td>

### 🚬 Smoking Behavior
> 🔵 Non-smokers: **151** | Smokers: **93**<br/>
> 💜 Tipping patterns are **similar** between groups<br/>
> 🩵 Smokers show slightly more tip variability<br/>
> 🌸 Smoking status has **low predictive power**

</td>
</tr>
<tr>
<td>

### 📊 Correlation Discoveries
> 🔴 `total_bill ↔ tip`: **Strong (+0.68)**<br/>
> 🟠 `size ↔ total_bill`: **Moderate (+0.60)**<br/>
> 🟡 `size ↔ tip`: **Moderate (+0.49)**<br/>
> 🟢 Tip % weakly related to other variables

</td>
<td>

### 👤 Gender Observations
> 🔵 Males tip on average: **$3.09**<br/>
> 💜 Females tip on average: **$2.83**<br/>
> 🩵 Difference is **statistically minor**<br/>
> 🌸 Bill-payers are 64% Male, 36% Female

</td>
</tr>
</table>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:FF6B35,50:FFD700,100:00FF88&height=4" />
</div>

<h2>🎨 <span style="color:#FF6B35">Visualizations Gallery</span></h2>

<div align="center">

| # | 🖼️ Plot | 🎯 Purpose | 🌈 Chart Type |
|:-:|:-------:|:---------:|:------------:|
| 01 | ![Total Bill Distribution](plot_01_total_bill_distribution.png) | Spending pattern overview | Histogram + KDE |
| 02 | ![Tip Distribution](plot_02_tip_distribution.png) | Tipping behavior analysis | Histogram + KDE |
| 03 | ![Day Count Plot](plot_03_day_countplot.png) | Traffic by weekday | Count Plot |
| 04 | ![Smoker Count](plot_04_smoker_count.png) | Customer demographics | Count Plot |
| 05 | ![Scatter Plot](plot_05_scatter_bill_tip.png) | Bill-to-tip relationship | Scatter Plot |
| 06 | ![Gender Analysis](plot_06_gender_tip_analysis.png) | Gender tipping comparison | Bar + Violin |
| 07 | ![Time Analysis](plot_07_time_analysis.png) | Lunch vs Dinner behavior | Box + Violin |
| 08 | ![Tips by Day](plot_08_tips_by_day.png) | Daily tipping patterns | Box Plot |
| 09 | ![Smoker Analysis](plot_09_smoker_tip_analysis.png) | Smoker tip behavior | Box + Strip |
| 10 | ![Pairplot](plot_10_pairplot.png) | All-variable relationships | Pairplot |
| 11 | ![Heatmap](plot_11_correlation_heatmap.png) | Feature correlations | Heatmap |
| 12 | ![Day-Time Heatmap](plot_12_day_time_heatmap.png) | Avg spending by day & time | Pivot Heatmap |
| 13 | ![FacetGrid](plot_13_facetgrid.png) | Multi-group comparison | FacetGrid Scatter |

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:8B00FF,50:FF0080,100:FFD700&height=4" />
</div>

<h2>🏆 <span style="color:#8B00FF">Conclusion & Recommendations</span></h2>

### ✅ Key Conclusions

> **1.** 💰 There is a **strong positive correlation (+0.68)** between total bill and tip amount — encouraging higher spending is directly linked to higher tips.
>
> **2.** 🍽️ **Dinner service** consistently generates **higher revenue** than Lunch across all days of the week.
>
> **3.** 👥 **Party size** has a meaningful positive impact on both bill amount and tips — group dining drives revenue.
>
> **4.** 📅 **Weekends (Sat & Sun)** account for the majority of customer traffic and should be the primary focus for staffing and promotions.
>
> **5.** 🚬 Smoking status has **limited predictive power** on tipping behavior — it should not be used as a primary segmentation variable.
>
> **6.** 📊 The dataset is **high quality** — no missing values, no duplicates, and consistent categorical encoding.

### 📌 Business Recommendations

<div align="center">

| 🎯 Priority | 📌 Recommendation | 💡 Expected Outcome |
|:-----------:|:-----------------:|:-------------------:|
| 🔴 **HIGH** | Launch weekend loyalty/rewards programs | Retain high-traffic weekend customers |
| 🟠 **HIGH** | Incentivize large group reservations | Higher per-visit revenue |
| 🟡 **MED** | Train staff on upselling dinner specials | Increase average bill size |
| 🟢 **MED** | Monitor high-value customers (bill > $40) | Build VIP loyalty tier |
| 🔵 **LOW** | Analyze tip percentage by season | Improve revenue forecasting |

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00BFFF,50:00FF88,100:FFD700&height=4" />
</div>

<h2>🚀 <span style="color:#00BFFF">Future Work & Improvements</span></h2>

### 🤖 Machine Learning Extensions

```python
# 🌈 Future ML Roadmap
future_work = {
    "Tip Prediction":      "LinearRegression, RandomForest, XGBoost",
    "Customer Clustering": "KMeans, DBSCAN, Hierarchical",
    "Revenue Forecasting": "ARIMA, Prophet, LSTM",
    "Anomaly Detection":   "IsolationForest, AutoEncoder"
}
```

<div align="center">

| 🧠 Area | 🔧 Technique | 🎯 Goal |
|:-------:|:------------:|:-------:|
| 🤖 **Regression** | XGBoost, Random Forest | Predict tip amount from features |
| 🎯 **Classification** | Logistic Regression, SVM | Predict if tip > 20% |
| 👥 **Clustering** | K-Means, DBSCAN | Segment customer profiles |
| 📈 **Forecasting** | Prophet, LSTM | Predict daily/weekly revenue |
| 🔍 **Hypothesis Testing** | ANOVA, t-test | Validate gender/smoking differences |
| 📊 **Dashboards** | Plotly Dash, Streamlit | Interactive real-time analytics |

</div>

### 📊 Advanced Statistical Methods

- **Hypothesis Testing** — ANOVA across days; t-test for gender differences
- **Confidence Intervals** — Bootstrap-based CI for average tip estimates
- **Regression Analysis** — Multiple linear regression with interaction terms
- **Chi-Square Tests** — Independence between categorical variables

### ☁️ Scalability & Deployment

```python
# 🚀 Deployment Pathways
deployment = [
    "☁️  AWS/GCP real-time restaurant data pipelines",
    "📊  Streamlit interactive EDA dashboard",
    "🔌  REST API for tip prediction service",
    "📱  Mobile-first analytics dashboard (Power BI)",
    "🤖  AutoML pipeline with MLflow tracking"
]
```

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF0080,25:FF6B35,50:FFD700,75:00FF88,100:00BFFF&height=180&section=footer&text=Thank%20You!&fontSize=42&fontColor=ffffff&fontAlignY=65&desc=Pandas%20%E2%80%A2%20NumPy%20%E2%80%A2%20Matplotlib%20%E2%80%A2%20Seaborn&descAlignY=85&descSize=16" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=700&size=18&pause=1500&color=FF0080&center=true&vCenter=true&width=800&lines=%F0%9F%8C%88+Transforming+Restaurant+Data+into+Actionable+Insights!;%F0%9F%9A%80+From+Raw+Numbers+to+Visual+Stories...;%F0%9F%93%8A+EDA+%7C+Statistics+%7C+Visualization+%7C+Machine+Learning" />

<br/><br/>

<img src="https://img.shields.io/badge/%F0%9F%8C%9F-Star%20this%20Repo-FF0080?style=for-the-badge" />
<img src="https://img.shields.io/badge/%F0%9F%94%81-Follow%20for%20More-8B00FF?style=for-the-badge" />
<img src="https://img.shields.io/badge/%F0%9F%92%AC-Open%20an%20Issue-00BFFF?style=for-the-badge" />

<br/><br/>

*✨ Built with ❤️ using Python, Pandas, NumPy, Matplotlib & Seaborn ✨*

</div>
