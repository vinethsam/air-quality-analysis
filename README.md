# Can We Predict and Explain Air Quality in Cities?

An interactive dashboard exploring air quality across Sri Lanka and major Asian cities. Covers 15 cities, 3 years of daily data, factor analysis, and a live AQI predictor.

**Author:** Vineth Samarasinghe
**Live Dashboard:** https://vinethsam.github.io/air-quality-analysis
**GitHub:** https://github.com/vinethsam/air-quality-analysis

---

## View It Live

No setup needed. The dashboard runs entirely in the browser.

---

## What This Project Covers

| Tab | What it shows |
|-----|--------------|
| Overview | City rankings, average AQI table, key stats |
| Interactive Map | Bubble map of all 15 cities with hover tooltips |
| Trends | Monthly AQI time series, seasonal breakdown, multi-city comparison |
| Factors | Monsoon effect, weekday vs weekend, seasonal patterns, key findings |
| AQI Predictor | Adjust weather sliders and get an instant AQI prediction |
| Model | R2, MAE, RMSE for Linear Regression and Random Forest, feature importance |

---

## Cities Covered

Sri Lanka: Colombo, Kandy

India: Delhi, Mumbai

China: Beijing, Shanghai

Southeast Asia: Bangkok, Jakarta, Kuala Lumpur, Singapore, Manila, Hanoi

South Asia: Dhaka, Karachi, Kathmandu

---

## Key Findings

**Dhaka and Delhi are the most consistently polluted cities**, averaging above 130 AQI year-round, with winter peaks regularly hitting Unhealthy levels.

**Singapore and Kandy are the standouts for clean air**, both averaging below 55 AQI across the full dataset.

**The monsoon effect is measurable**, with cities like Delhi and Bangkok dropping 20-35 AQI points during monsoon months as rainfall washes particulates from the air.

**Wind is the strongest weather predictor**, with a 5 m/s increase in wind speed associated with roughly a 10-15 point AQI reduction across all cities.

**Both models achieve R2 of 0.93**, explaining 93% of AQI variance. PM2.5 accounts for 78% of feature importance by a wide margin.

---

## Tech Stack

- Vanilla JavaScript and HTML, no framework needed
- Chart.js for all charts and visualisations
- SVG map with custom equirectangular projection
- Data pre-processed in Python (pandas, scikit-learn) and embedded directly in the page
- Hosted on GitHub Pages, one link, zero setup

---

## How to Run Locally

```bash
git clone https://github.com/vinethsam/air-quality-analysis.git
cd air-quality-analysis
# Open index.html in any browser
```

---

## Project Structure

```
air-quality-analysis/
+-- index.html        # The entire dashboard, self-contained
+-- data.json         # Pre-processed city and trend data
+-- README.md
```

---

## What I Would Add Next

- Live data via OpenWeatherMap API (free tier, 15 cities would need 15 calls per refresh)
- A 7-day AQI forecast using time series modelling
- Historical heatmap per city showing pollution by day of year
- Health impact calculator based on WHO thresholds
