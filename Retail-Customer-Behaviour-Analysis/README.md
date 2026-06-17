# 🛒 Shopping Trends Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on an e‑commerce shopping trends dataset to understand customer behavior, spending patterns, demographics, shipping preferences, and payment methods.  
The goal is to extract **business‑ready insights** that can support marketing, pricing, and customer retention strategies.

---

## 📂 Repository Structure
```
📁 Shopping-Trends-EDA/
│── EDA_Shopping_Trends.ipynb
│── shopping_trends.csv
│── README.md
```

---

## 🧰 Tools & Libraries Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

---

## 🧹 Data Preparation
- Removed missing or inconsistent values  
- Standardized categorical variables (gender, shipping type, payment method)  
- Verified numerical ranges for age, ratings, and purchase amounts  

---

## 🔍 Analysis & Visualizations
The notebook includes:

- **Purchase Amount vs Review Rating**  
- **Shipping Type Distribution**  
- **Gender Distribution**  
- **Payment Method Frequency**  
- **Product Category Trends**  
- **Subscription Status**  
- **Category vs Purchase Amount (Boxplot)**  
- **Age Distribution**  

---

## 💡 Key Business Insights
- Higher review ratings generally correspond to higher total purchase value  
- Certain shipping types dominate, indicating preferred logistics channels  
- A small number of product categories drive most sales  
- Subscription users represent a stable customer base  
- Most purchases come from a specific working‑age demographic  

---

## ▶️ How to Run
```bash
pip install pandas matplotlib seaborn numpy
jupyter notebook EDA_Shopping_Trends.ipynb
```

---

## 🛠 Troubleshooting
- Ensure the CSV file path matches the notebook  
- If plots do not appear, enable `%matplotlib inline`  
- Verify all libraries are installed  

---

## 🤝 Contributions
Contributions are welcome via pull requests.

---

## 📜 License
MIT License
