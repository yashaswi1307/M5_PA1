# Coupon Acceptance Analysis
Will the Customer Accept the Coupon?

## Overview

This project analyzes the drivers' acceptance of various coupon types based on demographic and situational patterns, and behaviors such as bar‐visiting frequency and destination urgency.

## Dataset

* **Source**: Repository ("Coupons" dataset)
* **Records**: 12,684 entries
* **Columns**: 26
* **Attributes**: (`age`, `gender`, `maritalStatus`, `income`, `occupation`), context (`destination`, `weather`, `temperature`, `time`), behavior (`passanger`, `Bar`, `CoffeeHouse`, `CarryAway`, `RestaurantLessThan20`, `Restaurant20To50`), coupon details (`coupon`, `expiration`, `toCoupon_GEQ5min`, etc.), and outcome (`Y` = accepted).

## Prerequisites

This project is designed to run in a Codio cloud workspace with full Jupyter Notebook and Python support. No local setup is required.

* **Codio Workspace**: Create or import this repository into a Codio project.
* **Python Environment**: Codio provides Python 3.x by default.
* **Notebook Server**: Launch Jupyter Notebooks directly from the Codio sidebar.

## Project Structure

```
├── data/
│   └── coupons.csv      # Raw dataset
├── analysis.ipynb       # Jupyter notebook with data cleaning, visualizations and analysis
└── README.md            # Project overview and instructions
```

## Usage

1. **Clone or download** the repository.
2. **Create** new Jupyter project.

#### From the Codio menu
1. Select **File > New Folder** (data folder)
2. **Place** `coupons.csv` in the `data` folder. (Select **File > Upload...**)
3. **Place** `analysis.ipynb` in the project root. (Select **File > Upload...**)
4. **Run** the notebook cells sequentially to reproduce data cleaning, exploration, and visualizations.

## Analysis Steps

1. **Data Inspection**: Load data, identify missing or problematic data, cleanup data (drop, compute etc. as appropriate).
2. **Statistics**: Compute overall acceptance rates and proportions.
3. **Visualization**:

   * Bar plots for Coupon Types Distribution
   * Histograms for temperature distribution
4. **Analysis**:

   * Investigating the Bar Coupons on various factors such as times of visits, age, maritalStatus, occupation, passengers, income
   * Investigating the Coffee House Coupons on various factors such as weather, passenger, destination
   * Age, income, destination, and weather-based comparisons
5. **Hypothesis Generation**: Make observations on which types of drivers most likely to redeem coupons (e.g., social outings for Coffee House coupons, frequent bar-goers for Bar coupons).

## Key Findings

* **Overall Acceptance**: \~56.8% of coupons accepted.
* **Bar Coupons**: Higher uptake among frequent bar-goers (>3 times/month).
* **CoffeeHouse Coupons**: Redeemed mainly during social, leisurely trips in rainy weather.

## Author

Yashaswi Raval

---

*For questions or contributions, please open an issue or submit a pull request.*

