# Data_Analysis_Project
# Life Expectancy Analysis in Africa (World Bank Data)

## Project Overview

This project analyzes **life expectancy trends across African countries** using data from the **World Bank**. The goal is to better understand how life expectancy has evolved over time and how it varies between countries, helping highlight disparities and long-term development patterns.

The analysis is implemented in Python using an **object-oriented approach**, making the code modular, reusable, and easy to extend.

---

## Problem Being Solved

Life expectancy is a key indicator of a country’s health system, economic development, and overall quality of life. However:

* Life expectancy varies significantly between African countries
* Trends over time are not always obvious from raw data
* Large datasets can be difficult to analyze without proper structure

**This project solves these issues by:**

* Cleaning and structuring World Bank life expectancy data
* Analyzing trends across countries and years
* Visualizing results to make insights easier to understand

---

## Object-Oriented Design

The project follows an **object-oriented design (OOD)** to organize responsibilities clearly.

### Main Classes and Responsibilities

#### I `DataLoader`

**Role:** Handles data loading and preprocessing

* Loads the World Bank dataset
* Filters African countries
* Cleans missing or invalid values

**Key Attributes:**

* `data`: Pandas DataFrame containing raw or cleaned data

**Key Methods:**

* `load_data()`
* `clean_data()`

---

#### II `LifeExpectancyAnalyzer`

**Role:** Performs statistical analysis

* Computes averages and trends
* Compares countries and regions

**Key Attributes:**

* `clean_data`: Processed dataset

**Key Methods:**

* `calculate_average_life_expectancy()`
* `trend_by_country(country)`

---

#### III `Visualizer`

**Role:** Displays insights visually

* Generates line charts and comparisons

**Key Methods:**

* `plot_trends()`
* `plot_country_comparison()`

---

### Relationships Between Classes

* `DataLoader` → provides cleaned data
* `LifeExpectancyAnalyzer` → consumes cleaned data for analysis
* `Visualizer` → uses analysis results to generate plots

This separation of concerns improves readability, maintenance, and scalability.

---

## How to Run the Program

### Prerequisites

Make sure you have **Python 3.8+** installed and the following libraries:

```bash
pip install pandas matplotlib seaborn numpy
```

### Steps to Run

1. Clone the repository:

```bash
git clone <repository-url>
cd <repository-folder>
```

2. Open the Jupyter Notebook:

```bash
jupyter notebook Life_Expectancy_Analysis_Africa_WB.ipynb
```

3. Run all cells from top to bottom to:

* Load the data
* Perform analysis
* Display visualizations

---

## Output

* Cleaned and structured datasets
* Statistical summaries of life expectancy
* Graphs showing trends across African countries

---

## Future Improvements

* Add more health indicators (mortality rate, healthcare spending)
* Integrate machine learning for prediction
* Build a web dashboard for interactive exploration

---

