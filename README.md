# 💼 VC Investment Data Analysis & Visualization

This project explores venture capital (VC) investment trends using a cleaned dataset of startup funding rounds. The analysis was performed using **PostgreSQL**, and results were visualized using **Tableau Public**.

---

## 📊 Project Goals

- Identify top-funded countries
- Understand funding trends by year
- Discover markets with the highest average funding
- Rank funding types by popularity
- Highlight top-funded companies

---

## 🛠️ Tools Used

- **PostgreSQL**: Data cleaning & querying
- **pgAdmin**: SQL interface for PostgreSQL
- **Python**: Used for data preprocessing (optional, not included in this repo)
- **Tableau Public**: Interactive visualizations and dashboards
- **CSV**: Exported SQL results for Tableau

---

## 🧮 Key SQL Queries

Here are examples of the queries used:

🔹 Top Countries by Total Funding
```sql
SELECT country_code, SUM(funding_total_usd_clean) AS total_funding
FROM investments
WHERE funding_total_usd_clean IS NOT NULL
  AND country_code IS NOT NULL AND country_code != ''
GROUP BY country_code
ORDER BY total_funding DESC
LIMIT 10;

---
```

📈 Visualizations in Tableau
The following charts were created:
[View Tableau Dashboard](https://public.tableau.com/app/profile/lita/viz/InvestmentDashboard_17506958718800/InvestmentDashboard?publish=yes)
![Investment Dashboard](https://github.com/user-attachments/assets/5bf13676-f7e5-4d7b-be2d-971b920cf709)

---

🧷 Credits

📂 Dataset: [VC Investment (Kaggle)](https://www.kaggle.com/datasets/arindam235/startup-investments-crunchbase)

💻 Author: Lita

🗓 Date: June 2025

---

📎 Connect With Me

🌐 [LinkedIn](https://www.linkedin.com/in/lita-utami-wulandari/)

💼 [GitHub](https://github.com/litascripts)

📧 Email: litautamiwulandari@gmail.com

