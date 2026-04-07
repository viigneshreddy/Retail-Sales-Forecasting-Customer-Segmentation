# Retail-Sales-Forecasting-Customer-Segmentation
# RetailIQ — Sales Forecasting & Customer Intelligence Dashboard

![RetailIQ Dashboard](https://img.shields.io/badge/RetailIQ-Dashboard-f0b429?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)

## Overview

**RetailIQ** is a single-page, interactive business intelligence dashboard for retail sales analysis, demand forecasting, and customer segmentation. Built entirely with vanilla HTML, CSS, and JavaScript, it requires no backend or build tools — just open the file in a browser and explore.

The dashboard uses **synthetic data** to demonstrate real-world analytical techniques used in retail analytics, making it a great reference for data visualization, forecasting methods, and customer intelligence concepts.

---

## Live Features

### 📊 Overview Tab
- **Monthly Revenue Chart** — 12-month revenue trend with seasonal patterns
- **Revenue by Category** — Donut chart breaking down 5 product categories (Electronics, Apparel, Home Goods, Food & Bev, Sports)
- **Weekly Sales Heatmap** — Stacked bar chart showing sales volume by day of week across all months
- **Key Insights Panel** — Auto-generated narrative insights highlighting Q4 spikes, top categories, weekend uplift, and seasonal dips

### 📈 Forecasting Tab
- **24-Month Forecast** — Triple Exponential Smoothing (Holt-Winters) model with 95% confidence bands
- **Interactive Controls** — Adjust the smoothing factor (α) and seasonality strength in real-time
- **Model Performance Metrics** — Live MAPE, RMSE, trend rate, and seasonality index
- **Seasonality Decomposition** — Visual breakdown of Trend, Seasonal, and Residual components
- **Forecasting Methods Comparison** — Side-by-side MAPE and complexity comparison: Naive, Moving Average, Exp. Smoothing, Holt-Winters, ARIMA, and Prophet

### 👥 Segmentation Tab
- **RFM Customer Clustering** — K-Means (k=5) bubble scatter plot on Recency vs. Frequency axes
- **Segment Distribution Donut** — Visual breakdown of 8,340 synthetic customers across 5 segments
- **Segment Profiles Table** — Detailed per-segment stats: customer count, avg spend, purchase frequency, revenue share, recency, and recommended strategy

### 💡 Concepts Tab
- Plain-language explanations of all analytical methods used: Time Series Forecasting, RFM Segmentation, K-Means Clustering, MAPE, Seasonality Decomposition, and Actionable Segmentation
- **Model Selection Radar Chart** — Multi-axis comparison of Holt-Winters, ARIMA, Prophet, and Moving Average across accuracy, interpretability, speed, and ease of use

---

## KPI Strip

| Metric | Value |
|--------|-------|
| Total Revenue (12mo) | $4.82M (+12.4% YoY) |
| Active Customers | 8,340 (+8.1% growth) |
| Avg Order Value | $142 (-2.3% YoY) |
| Forecast Accuracy | 91.2% (MAPE 8.8%) |

---

## Tech Stack

| Technology | Purpose |
|------------|---------|
| HTML5 / CSS3 | Layout, styling, animations |
| Vanilla JavaScript | Data generation, logic, interactivity |
| [Chart.js 4.4.1](https://www.chartjs.org/) | All charts and visualizations |
| [Google Fonts](https://fonts.google.com/) | Syne, DM Mono, Lora typefaces |

> No frameworks, no bundlers, no dependencies to install.

---

## Getting Started

### Option 1 — Open Directly
```bash
# Clone the repo
git clone https://github.com/viigneshreddy/<your-repo-name>.git

# Open in your browser
open index.html
```

### Option 2 — Serve Locally (recommended for full font loading)
```bash
# Using Python
python -m http.server 8080

# Then visit
http://localhost:8080
```

---

## Project Structure

```
├── index.html        # All-in-one dashboard (HTML + CSS + JS)
└── README.md
```

---

## Analytical Methods Used

### Holt-Winters Triple Exponential Smoothing
The forecasting engine uses Holt-Winters with three smoothing parameters:
- **α (Alpha)** — Level smoothing (adjustable via slider: 0.1–0.9)
- **β (Beta)** — Trend smoothing (fixed at 0.1)
- **γ (Gamma)** — Seasonal smoothing (fixed at 0.3)
- **Season length** — 12 months

### RFM Segmentation
Customers are scored on Recency, Frequency, and Monetary value, then clustered into 5 segments:

| Segment | Strategy |
|---------|----------|
| ⭐ Champions | Reward & referral programs |
| 💎 Loyal | Loyalty VIP tiers |
| 🌱 Potential | Targeted upsell emails |
| ⚠️ At-Risk | Win-back campaigns |
| 💤 Lapsed | Reactivation with incentive |

---

## Data Note

All data in this dashboard is **synthetically generated** using a seeded pseudo-random number generator. The patterns (seasonal peaks, trends, customer distributions) are designed to reflect realistic retail behavior but do not represent any real company or dataset.

---

## Use Cases

- Portfolio project showcasing data visualization and analytics
- Teaching aid for retail analytics, forecasting, and CRM concepts
- Starting template for a real-world BI dashboard
- Interview prep for data analyst / BI developer roles

---

## Contributing

1. Fork this repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

*Built with Chart.js · Powered by synthetic data · No backend required*
