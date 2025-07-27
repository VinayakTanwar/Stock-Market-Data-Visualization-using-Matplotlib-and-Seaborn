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

