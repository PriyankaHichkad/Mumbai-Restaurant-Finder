---
TITLE: Mumbai-Restaurant-Finder
AUTHOR: Priyanka Rajeev Hichkad
---

# Mumbai Restaurant Insights: A Data-Driven Exploration

## Project Overview

This project is a personal initiative to combine two of my strongest interests — food and data. The objective is to build an **interactive dashboard** that helps users explore and identify top-rated restaurants in Mumbai based on their **location** and **cuisine preferences**. 

The process involves:
- Cleaning and preparing a restaurant dataset using Python
- Creating an interactive experience with Power BI
- Enabling intuitive food discovery backed by data

As a food enthusiast who often searches for the perfect late-night bite, a weekend brunch spot, or even a new bakery to try, I wanted a more data-driven and organized way to make these choices. This project is both a professional data visualization exercise and a personal tool I find practical and meaningful.

---

## Dataset Description

The dataset is sourced from [Kaggle](https://www.kaggle.com/) : [https://www.kaggle.com/datasets/sleepyowl007/zomato-mumbai-dataset/data](https://www.kaggle.com/datasets/sleepyowl007/zomato-mumbai-dataset/data) (search for `zomato_mumbai_dataset.csv`) and includes the following fields:
- Restaurant name
- Address and locality
- Cuisines provided
- Price range
- User ratings
- Review sentiments
- Number of votes
- Timings
- Zomato URL

> **Note:** The dataset is approximately **four years old**. While it’s still great for insights, some restaurants may have changed or closed over time. Always cross-check real-time availability if using this as a restaurant finder.

---

## Data Cleaning and Preprocessing

The raw dataset required a number of transformations before analysis. The following key steps were performed in the Jupyter Notebook:

- **Duplicate Removal**: Ensured only unique restaurant entries are retained.
- **Null Handling**: Cleaned missing fields in columns like reviews, cuisines, and timing.
- **Review Label Encoding**: Standardized multilingual review values into consistent categories.
- **Text Normalization**: Cleaned address and cuisine fields for uniform filtering.
- **Categorical Formatting**: Reformatted key categorical variables for smooth integration with Power BI slicers.

The cleaned dataset was exported as a CSV and used in Power BI for visualization.

---

## Dashboard Walkthrough

### 🔍 Slicers (Interactive Filters)

The dashboard provides two primary slicers for user interaction:

1. **"Where are you?"** – Filters the dataset based on the selected locality in Mumbai (e.g., Andheri, Bandra, Powai).
2. **"Your taste"** – Filters based on cuisine type (e.g., Chinese, Fast Food, Bakery, Bar, North Indian, etc.).

### 📊 Visualizations

After selecting your location and preferred cuisine type:

- A **histogram** appears showing up to **10 top-rated restaurants** that match your criteria:
  - **X-axis**: Restaurant names
  - **Y-axis**: Average user ratings

- **Insight cards** display:
  - Average price for two
  - Number of votes
  - Average review sentiment
  - Detailed list of cuisines offered by the selected restaurants

---

## 📷 Dashboard Screenshots

![Dashboard Overview](https://github.com/PriyankaHichkad/Mumbai-Restaurant-Finder/blob/main/Dashboard%20Screenshot.png)
