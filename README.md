# 🌧️ Rainfall in India Analysis (1901–2015) – Power BI Dashboard

An interactive **Power BI dashboard** analyzing more than a century of rainfall data across Indian regions.  
This project explores **long-term rainfall trends, seasonal patterns, geographic distribution, and climate variability** using data visualization and analytical storytelling.

---

# 📊 Project Overview

India's rainfall patterns are heavily influenced by seasonal monsoons and regional geography.  
Understanding rainfall trends is important for **agriculture, water resource planning, and climate research**.

This project analyzes rainfall data from **1901 to 2015** across Indian subdivisions to uncover:

- Long-term rainfall trends
- Regional rainfall disparities
- Seasonal rainfall patterns
- Monsoon dependency
- Extreme rainfall events
- Climate variability using anomaly analysis

The dashboard presents these insights through **interactive Power BI visualizations**.

---

# 🗂 Dataset

Dataset: **Rainfall in India (1901–2015)**

Source: Kaggle / Meteorological datasets

### Key Features

| Column | Description |
|------|-------------|
| SUBDIVISION | Indian geographical region |
| YEAR | Year of observation |
| JAN – DEC | Monthly rainfall (mm) |
| ANNUAL RAIN | Total rainfall for the year |
| WINTER RAIN | Jan–Feb rainfall |
| PRE MONSOON RAIN | Mar–May rainfall |
| MONSOON RAIN | Jun–Sep rainfall |
| POST MONSOON RAIN | Oct–Dec rainfall |

The dataset contains **115 years of rainfall records across multiple Indian subdivisions**.

---

# 🛠 Tools & Technologies

- **Power BI Desktop**
- Data Modeling
- DAX Measures
- Data Cleaning (Power Query)
- Data Visualization
- Climate Trend Analysis

---

# 📈 Dashboard Structure

The report is designed as a **story-driven analysis with four pages**.

---

# 1️⃣ Rainfall Overview

Provides a high-level understanding of India's rainfall patterns.

### Visuals

- Rainfall Trend (1901–2015)
- Key rainfall statistics (Average, Maximum, Minimum)
- Top 10 rainfall years
- Rainfall distribution

### Insights

- Rainfall fluctuates significantly year-to-year
- Certain years experience extreme rainfall
- Overall rainfall patterns remain relatively stable over long periods

---

# 2️⃣ Geographic Rainfall Distribution

Examines how rainfall varies across Indian regions.

### Visuals

- Rainfall map of India
- Top rainfall regions
- Regional rainfall comparison

### Insights

- Western Ghats and Northeast India receive the highest rainfall
- Northwestern regions receive significantly less rainfall
- Rainfall distribution across India is highly uneven

---

# 3️⃣ Seasonal Rainfall Patterns

Analyzes how rainfall is distributed across seasons.

### Visuals

- Seasonal rainfall contribution
- Seasonal rainfall trend over time
- Monsoon rainfall trend

### Insights

- Monsoon rainfall contributes **70–80% of annual rainfall**
- Winter rainfall is minimal
- Pre-monsoon and post-monsoon rainfall vary by region

---

# 4️⃣ Climate Trends & Variability

Investigates long-term rainfall patterns and anomalies.

### Visuals

- Decade-wise rainfall trend
- Rainfall variability analysis
- Monsoon dependency by region
- Rainfall anomaly chart

### Insights

- Rainfall varies significantly across decades
- Some years experience strong positive or negative rainfall anomalies
- Certain regions rely heavily on monsoon rainfall

---

# 📊 Key Analytical Techniques

### Rainfall Anomaly Analysis

Rainfall anomaly measures how much rainfall deviates from the long-term average.

DAX Example:

```DAX
Yearly Avg Rainfall = AVERAGE('RAINFALL'[ANNUAL RAIN])

Long Term Avg Rainfall =
CALCULATE(
    AVERAGE('RAINFALL'[ANNUAL RAIN]),
    ALL('RAINFALL'[YEAR])
)

Rainfall Anomaly =
[Yearly Avg Rainfall] - [Long Term Avg Rainfall]

```


This helps identify:
- Drought years
- Extreme rainfall years
- Climate variability patterns

# 📌 Key Findings
- The monsoon season dominates India's rainfall, contributing the majority of annual precipitation.
- Rainfall distribution across India is geographically uneven.
- Long-term rainfall trends show variability but no consistent linear increase or decrease.
- Several years exhibit extreme rainfall anomalies, highlighting climate variability.

# 📂 Project Structure
```python 
Rainfall-India-PowerBI-Dashboard
│
├── Rainfall.pbix
├── rainfall_in_india_1901_2015.csv
└── README.md
```

# 🚀 How to Use
- Download the .pbix file
- Open using Power BI Desktop
- Interact with filters and slicers
- Explore rainfall insights across regions and seasons

# 👤 Author
Rahul Agarwal
B.Tech – Computer Science & Engineering
MANIT Bhopal
