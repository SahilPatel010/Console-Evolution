# The Console Wars: A Data Visualization Project

## Project Overview

This project provides a data-driven look at the "Console Wars" by visualizing global video game sales for major platforms from 1995 to 2016. The goal was to take a large, raw dataset and transform it into a clear and insightful stacked area chart that tells the story of market trends and competition in the gaming industry.

This project demonstrates skills in data cleaning, aggregation, transformation with Pandas, and advanced visualization with Matplotlib and Seaborn.

---

## The Analysis Process

The Jupyter Notebook (`VideoGamesStackedChart (2).ipynb`) in this repository details the following steps:

1.  **Data Loading and Cleaning:**
    * The dataset, containing over 16,000 video game records, was loaded using Pandas.
    * Rows with missing `Year` values were identified and dropped to ensure data integrity.

2.  **Data Filtering and Selection:**
    * The data was filtered to the years 1995-2016 to focus on the modern era of console gaming.
    * To keep the chart readable, the analysis was focused on the **top 6 best-selling platforms** of all time.

3.  **Data Transformation:**
    * The core of the project involved using `.groupby()` to aggregate total `Global_Sales` for each `Platform` and `Year`.
    * The `.unstack()` method was then used to pivot the data, creating a table with years as the index and platforms as columns—the perfect format for a stacked area chart.

4.  **Data Visualization:**
    * A stacked area chart was created using **Matplotlib** to visualize the sales data over time.
    * The chart was styled professionally with a clear title, labeled axes, a legend, and an alpha transparency for better readability.
    * A key formatting step was implemented to ensure the x-axis (Year) displayed only integer values, making the chart clean and professional.

---

## How to Use This Repository

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    ```
2.  **View the Notebook:**
    * Open `VideoGamesStackedChart (2).ipynb` to see the full Python code and step-by-step process.
3.  **See the Final Chart:**
    * `console_wars_chart.png` is the final visualization created by the notebook.
4.  **Explore the Data:**
    * `vgsales.csv` is the original dataset used for the analysis.

---

## Tools and Libraries

* **Python 3**
* **Pandas:** For data loading, cleaning, and transformation.
* **Matplotlib & Seaborn:** For data visualization.
* **Jupyter Notebook:** For interactive analysis and documentation.
