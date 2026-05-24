<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=300&color=gradient&customColorList=24,12,20,17,30,6&text=SEABORN%20TIPS%20DATA%20ANALYSIS&fontSize=45&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Pandas%20•%20NumPy%20•%20Matplotlib%20•%20Seaborn&descAlignY=60"/>

<br>

<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=800&size=30&duration=2500&pause=1000&color=FF0000&center=true&vCenter=true&multiline=true&repeat=true&width=1200&height=120&lines=📊+SEABORN+TIPS+DATASET+ANALYSIS;🚀+Exploratory+Data+Analysis+(EDA);📈+Visualizations+%7C+Insights+%7C+Statistics;🌈+Built+With+Pandas+NumPy+Matplotlib+Seaborn"/>

<br>

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
<img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge"/>

</div>

---

<div align="center">

# 🌈✨ DATA ANALYSIS REPORT ✨🌈

<img src="https://user-images.githubusercontent.com/74038190/216656986-9e8f8e0f-3b31-4f41-a0f0-00a34b9cb2b6.gif" width="100%">

</div>

---

# 🎯 OBJECTIVE

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Poppins&weight=700&size=24&pause=1000&color=00FFFF&center=true&vCenter=true&width=900&lines=Understanding+Restaurant+Customer+Behaviour;Analyzing+Bills+Tips+and+Spending+Patterns;Discovering+Hidden+Insights+Through+EDA"/>

</div>

> 🌟 The Tips Dataset is a popular Seaborn dataset containing information about restaurant bills, tips, customer demographics, dining times, and party sizes.

---

# 🌈 DATASET OVERVIEW

<table>
<tr>
<td width="50%">

### 📦 Dataset Shape

```python
tips.shape
```

Output

```python
(244,7)
```

</td>

<td width="50%">

### 📝 Features

| Feature | Description |
|----------|-------------|
| total_bill | Total bill amount |
| tip | Tip amount |
| sex | Gender |
| smoker | Smoker status |
| day | Weekday |
| time | Lunch/Dinner |
| size | Party size |

</td>
</tr>
</table>

---

# 📊 VISUALIZATION SHOWCASE

<div align="center">

## 🌈 Distribution Analysis

![Distribution](plots/distribution.png)

---

## 🔥 Correlation Heatmap

![Heatmap](plots/heatmap.png)

---

## 🚀 Scatter Plot Analysis

![Scatter](plots/scatter.png)

---

## ✨ Pairplot Analysis

![Pairplot](plots/pairplot.png)

</div>

---

# 📈 EXPLORATORY DATA ANALYSIS

## 🌈 Distribution Plot

```python
plt.figure(figsize=(12,6))

sns.histplot(
    data=tips,
    x="total_bill",
    kde=True,
    bins=20,
    color="purple"
)

plt.title(
    "Distribution of Total Bills",
    fontsize=18,
    fontweight="bold"
)

plt.show()
```

![Total Bill Distribution](plots/total_bill_distribution.png)

---

## 🔥 Correlation Heatmap

```python
corr = tips.corr(
    numeric_only=True
)

plt.figure(figsize=(10,6))

sns.heatmap(
    corr,
    annot=True,
    cmap="rainbow",
    linewidths=2
)

plt.show()
```

![Correlation Heatmap](plots/correlation_heatmap.png)

---

# 💡 KEY INSIGHTS

<table>
<tr>
<td>

### 💰 Spending Trends

- Most bills range between \$10–\$25
- Few high-value bills exceed \$40
- Spending distribution is right-skewed

</td>

<td>

### 🍽 Dining Patterns

- Dinner customers spend more
- Weekend traffic is highest
- Larger groups create larger bills

</td>
</tr>
</table>

---

## 🚀 Major Findings

✨ Higher bills generate larger tips

✨ Dinner contributes maximum revenue

✨ Weekend customers dominate traffic

✨ Larger groups spend significantly more

✨ Positive correlation exists between bill and tip

---

# 🎨 TECHNOLOGY STACK

<div align="center">

<img src="https://skillicons.dev/icons?i=python"/>

<br><br>

<img src="https://img.shields.io/badge/Pandas-FF0080?style=for-the-badge&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-00FFFF?style=for-the-badge&logo=numpy&logoColor=black"/>
<img src="https://img.shields.io/badge/Matplotlib-FF6600?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Seaborn-9933FF?style=for-the-badge"/>

</div>

---

# 🔮 FUTURE SCOPE

### 🤖 Machine Learning

- Tip Prediction
- Revenue Prediction
- Customer Segmentation



### ☁ Advanced Analytics

- Regression Analysis
- Hypothesis Testing
- ANOVA
- Forecasting Models

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=200&section=footer&color=gradient&customColorList=24,12,20,17,30,6"/>

<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=800&size=28&duration=3000&pause=1000&color=39FF14&center=true&vCenter=true&width=900&lines=THANK+YOU+FOR+VISITING;DATA+ANALYSIS+PROJECT;PANDAS+•+NUMPY+•+MATPLOTLIB+•+SEABORN"/>

### ⭐ If you like this project, consider giving it a star ⭐

</div>
