# # 🎮 Video Game Sales Forecasting Using Python & Prophet

A complete time series forecasting project analyzing and predicting global and regional video game sales from **1971 to 2024** using Python and Prophet. 
The project utilizes real-world data from [Maven Analytics](https://mavenanalytics.io/data-playground).

---

## 📁 Dataset Overview

* **Source**: Maven Analytics - Video Game Sales
* **Total Records**: 62,884 games
* **Time Span**: 1971–2024
* **Fields**:

  * `title`, `console`, `genre`, `publisher`, `developer`
  * `critic_score`, `total_sales`, `na_sales`, `jp_sales`, `pal_sales`, `other_sales`
  * `release_date`, `last_update`

---

## 🎯 Project Objectives

1. Clean and preprocess the video game dataset
2. Handle missing values with smart imputation
3. Perform **Time Series Forecasting** using Prophet
4. Forecast future sales:

   * Globally
   * Region-wise (NA, JP, PAL, Other)
   * Genre-wise (Top 5 Genres)
5. Visualize trends using Matplotlib
6. Summarize insights and business takeaways

---

## 🧪 Tools & Libraries Used

* **Python**

  * `Pandas`, `NumPy` – Data wrangling
  * `Prophet` – Time series modeling
  * `Matplotlib`, `Seaborn` – Visualizations

---

## 🔍 Data Cleaning Highlights

* Dropped columns with excessive nulls (e.g., image URLs, last update)
* Extracted `release_year` from `release_date`
* Replaced missing numerical values using **genre-wise mean imputation**
* Final dataset size after cleaning: **56,954 records**

---

## 📈 Forecasting Insights

### 1. **Global Sales Forecast**

* Clear upward trend projected beyond 2024
* Moderate growth expected with seasonal uncertainty

### 2. **Region-wise Forecasts**

| Region | Insight                          |
| ------ | -------------------------------- |
| NA     | Remains the most dominant market |
| JP     | Stagnant or declining            |
| PAL    | Stable and slowly rising         |
| Other  | Shows emerging potential         |

### 3. **Genre-wise Forecasts (Top 5 Genres)**

* **Action** and **Sports** games continue to grow
* **Adventure** and **Miscellaneous** genres show consistent performance
* Graphs show strong seasonality and growth patterns

---

## 📊 Visual Examples

> You can find all plots in the `graphs/` directory.

![Sample Forecast](graphs/forecast_action.png)

---

## ✅ Project Status

* [x] Data cleaning & preprocessing
* [x] Prophet-based forecasts (global, regional, genre-wise)
* [x] Graph labeling and export
* [ ] Power BI dashboard (in progress)

---

## 💡 Business Takeaways

* Action games are a consistent top-seller and show future growth potential
* Japan’s video game market may require revitalization strategies
* Other regions are rising and may offer untapped opportunities

---
