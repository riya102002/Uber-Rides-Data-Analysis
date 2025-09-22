# Uber Rides Data Analysis 🚗💨

![Language](https://img.shields.io/badge/Language-Python-blue.svg)
![Pandas](https://img.shields.io/badge/Library-Pandas-orange.svg)
![Seaborn](https://img.shields.io/badge/Library-Seaborn-purple.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

A comprehensive analysis of an Uber rides dataset to uncover key insights into travel patterns, peak usage times, and operational factors. This project serves as a demonstration of a complete data analysis workflow, from cleaning and feature engineering to visualization and insight generation.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Tools and Libraries](#tools-and-libraries)
- [Analysis Workflow](#analysis-workflow)
- [Key Insights and Findings](#key-insights-and-findings)
- [How to Run This Project](#how-to-run-this-project)
- [License](#license)

---

## Project Overview

This project performs an in-depth exploratory data analysis (EDA) on a dataset of Uber rides. The primary goal is to understand the behavior of the users in this dataset by analyzing various factors such as trip purpose, time of day, day of the week, and popular routes. By cleaning the data, engineering new features, and creating insightful visualizations, we paint a clear picture of the service's usage patterns, revealing a profile heavily skewed towards business-related travel.

---

## Dataset

The dataset used is **`UberDataset.csv`**. It contains anonymized information about individual Uber trips, including:
- **`START_DATE` and `END_DATE`**: Timestamps for the beginning and end of each trip.
- **`CATEGORY`**: The category of the trip (Business or Personal).
- **`START` and `STOP`**: The start and end locations of the trip.
- **`MILES`**: The distance of the trip.
- **`PURPOSE`**: The purpose of the trip (e.g., Meeting, Meal/Entertain).

---

## Tools and Libraries

This project is built within a Jupyter Notebook environment and leverages the following core Python libraries:
- **Python**
- **Pandas:** For data manipulation, cleaning, and aggregation.
- **NumPy:** For numerical operations.
- **Matplotlib & Seaborn:** For creating a wide range of static data visualizations.

---

## Analysis Workflow

The analysis was conducted in a structured manner, following these key steps:

1.  **Data Cleaning and Preprocessing:** Handled missing values (especially in the `PURPOSE` column), converted date columns to the correct `datetime` format, and removed duplicate entries to ensure data quality.
2.  **Feature Engineering:** Created new, more insightful features from the existing data to enable deeper analysis. This included:
    - **Time-based features:** `HOUR`, `DAY`, `MONTH`, `DAY_NIGHT`.
    - **Trip-based features:** `TRIP_DURATION_MIN`, `AVG_SPEED_MPH`, `ROUTE`.
3.  **Exploratory Data Analysis (EDA):** Performed a deep dive into the data using visualizations to identify trends, patterns, and outliers, leading to the key findings below.

---

## Key Insights and Findings 

The analysis of the dataset revealed several clear patterns that characterize the usage of the service:

* **Business-Focused Usage:** The service is predominantly used for **Business** purposes, with "Meetings" and "Meal/Entertain" being the most common reasons. This is reflected in the significantly lower usage on weekends.


* **Clear Temporal Patterns:** **Fridays** are the busiest day of the week, and the **afternoon** is the peak time for travel. This pattern strongly aligns with a typical business work week.

* **Predominantly Short-Distance:** The vast majority of trips are **short-haul**, typically under 10 miles. This indicates the service is primarily used for local travel between nearby destinations.

* **A Single, Dominant Corridor:** One route, **Cary to Morrisville**, emerged as the most frequently traveled by a large margin, highlighting a critical and regular travel path for users in this dataset.


* **Real-World Traffic Impact:** The analysis of average speed shows a clear **dip during afternoon hours**, which directly corresponds to peak traffic congestion. This demonstrates that real-world factors are visibly reflected in the data.


---

## How to Run This Project

To replicate this analysis on your own machine, follow these steps:

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/your-username/Uber-Rides-Analysis.git](https://github.com/your-username/Uber-Rides-Analysis.git)
    cd Uber-Rides-Analysis
    ```
2.  **Install Dependencies**
    It's recommended to create a virtual environment first. All required libraries are listed in the `requirements.txt` file.
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Jupyter Notebook**
    Launch Jupyter Notebook and open the `.ipynb` file to view and run the analysis.
    ```bash
    jupyter notebook "Uber Data Analysis.ipynb"
    ```

---

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.
