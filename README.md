# Los Angeles Airbnb Listings Analysis

## Overview

This project explores the Los Angeles Airbnb listings dataset (`listings.csv`) to uncover trends and insights within the short-term rental market. The analysis focuses on understanding the factors that contribute to a successful listing by examining host behavior, market dynamics, pricing strategies, and listing characteristics like property type and location.

## Dataset

The dataset used is a snapshot of Airbnb listings in Los Angeles, California, containing detailed information about properties, hosts, pricing, availability, and reviews.

*(Note: If you know the source or date of the dataset, you could add it here, e.g., "Dataset sourced from [Source Name/Inside Airbnb] as of [Date].")*

## Objectives

*   Perform comprehensive data cleaning and preprocessing on the raw listings data.
*   Analyze host characteristics and behavior, including response times, response rates, and the impact of Superhost status.
*   Conduct market analysis to understand pricing variations across neighborhoods, property types, and room types.
*   Investigate demand patterns through review volume, minimum night stays, and availability.
*   Identify key factors and combinations that correlate with highly-rated or frequently booked listings.

## Methodology

1.  **Data Loading & Initial Exploration:** Loaded the `listings.csv` dataset using Pandas and performed initial checks on data shape, types, and missing values.
2.  **Data Preprocessing:**
    *   Handled missing values through imputation (e.g., filling `host_response_rate` with 0, `host_is_superhost` with 'f') or removal (e.g., rows missing critical info like `name` or `price`).
    *   Corrected data types (e.g., converting date columns, boolean-like columns).
    *   Performed feature engineering by creating new columns like `has_reviews?` (boolean based on review score presence) and `days_hosting` (calculated from `host_since`).
3.  **Exploratory Data Analysis (EDA):**
    *   Analyzed host behavior patterns (response times vs. rates, Superhost comparisons).
    *   Examined market trends (price distributions, average prices by neighborhood/property/room type).
    *   Assessed listing demand (review volume by neighborhood, minimum nights by room type).
    *   Compared metrics between high-rated (>= 4.8) and lower-rated listings.
4.  **Visualization:** Used Seaborn and Matplotlib to create histograms, bar plots, box plots, scatter plots (map), and pie charts to visualize distributions and relationships.

## Key Findings

*   The majority of listings fall within the $101-$200 price range, which also sees the highest volume of reviews.
*   Superhosts demonstrate significantly higher response rates and receive more reviews and higher average ratings compared to non-Superhosts.
*   Entire homes/apartments are the most common and popular listing type, followed by private rooms.
*   Listings with higher ratings (>= 4.8) tend to have slightly lower average prices but receive significantly more reviews.
*   Host tenure correlates positively with both average price and average review scores.
*   Neighborhoods like Long Beach, Venice, and Santa Monica show high listing density and review volume, indicating strong demand.

## Technologies Used

*   Python 3
*   Jupyter Notebook
*   Pandas
*   Seaborn
*   Matplotlib

## How to View/Run

The complete analysis and visualizations are contained within the Jupyter Notebook: `project_python.ipynb`.

To run the notebook locally:
1.  Ensure you have Python and the necessary libraries (Pandas, Seaborn, Matplotlib) installed.
2.  Download the `project_python.ipynb` file and the `listings.csv` dataset.
3.  Place the `listings.csv` file in the same directory as the notebook.
4.  Launch Jupyter Notebook or JupyterLab and open `project_python.ipynb`.
5.  Run the cells sequentially.

---

*Author: Isaac Edem Adoboe*
*Date: Based on Notebook Metadata (e.g., December 2024)*
