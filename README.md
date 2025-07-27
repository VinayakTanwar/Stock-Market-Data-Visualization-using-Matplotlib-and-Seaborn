
````markdown
# 📊 Stock Market Data Visualization using Matplotlib and Seaborn

This is a mini data visualization project created using **Python**, **Pandas**, **Matplotlib**, and **Seaborn**.  
It explores stock data for multiple companies and visualizes trends, distributions, and comparisons in an easy-to-understand way.

---

## 🧾 Dataset

The dataset contains:
- **Company Names**
- **Dates**
- **Close Prices**
- **Volume Traded**

Each row represents stock data for a company on a particular date.

---

## 📌 Objectives

- Analyze closing price trends over time.
- Compare average closing prices of companies.
- Visualize volume and distribution of stock data.

---

## 📈 Visualizations Used

### Line Plot
Shows the closing price trend over time for each company.
```python
sns.lineplot(data=df, x='Date', y='Close', hue='Company')
````

### Bar Plot

Compare average closing prices by company.

```python
df.groupby('Company')['Close'].mean().plot(kind='bar')
```

### Box Plot

Shows spread and outliers in the closing price for each company.

```python
sns.boxplot(x='Company', y='Close', data=df)
```

### KDE Plot

Density distribution of close prices by company.

```python
sns.kdeplot(data=df, x='Close', hue='Company', fill=True)
```

### Violin Plot

Combines boxplot + KDE for volume analysis.

```python
sns.violinplot(x='Company', y='Volume', data=df)
```

### Count Plot

Number of records per company.

```python
sns.countplot(x='Company', data=df)
```

---

## 💻 Libraries Used

* Python
* Pandas
* Matplotlib
* Seaborn

---

## 📂 Project Structure

```
📁 stock-viz-project/
├── stock_data.csv           # Your dataset
├── stock_visualizations.ipynb  # Jupyter/Colab Notebook
└── README.md                # This file
```

---

## ✅ What I Learned

* Data cleaning and grouping using Pandas.
* Different types of Seaborn and Matplotlib plots.
* How to choose the right chart for the right question.
* Hands-on practice with real-world-like data.

---

## 🚀 Future Plans

* Add interactivity using Plotly.
* Add more financial KPIs like Open, High, Low.
* Try predictive modeling later (with machine learning).

---

## 📌 Author

**Vinayak Tanwar**
📍 BCA with AI & Data Science | Poornima University
🔗 [LinkedIn](https://www.linkedin.com/in/vinayaktanwar)

---

## 📝 License

This project is for learning purposes only.

