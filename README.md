# 🏠 New Zealand Airbnb ROI Analysis

![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
[![nbviewer](https://img.shields.io/badge/view%20on-nbviewer-brightgreen.svg)](https://nbviewer.jupyter.org/github/your-username/NZ-Airbnb-ROI-Analysis/blob/main/airroi_nz_simple_optimized.ipynb)

This project analyzes **Return on Investment (ROI)** for Airbnb vacation rentals in **Queenstown** and **Christchurch**, New Zealand, using data from the AirROI API. Covering August 2024–July 2025, it compares key metrics—active listings, occupancy rates, average daily rates (ADR), revenue, and revenue-to-median house price ratio—to guide property investment decisions. Visualizations highlight Queenstown’s tourism-driven peaks and Christchurch’s stable urban market.

**[View the notebook interactively](https://nbviewer.jupyter.org/github/renjij/NZ-Airbnb-ROI-Analysis/blob/main/airroi_nz_simple_optimized.ipynb)** or explore the code in this repository!

## 📋 Project Overview

This Jupyter notebook (`airroi_nz_simple_optimized.ipynb`) uses the AirROI API to fetch and analyze Airbnb market data for Queenstown (Otago) and Christchurch (Canterbury). Key objectives include:
- Comparing market performance (active listings, occupancy, ADR, revenue) over 12 months.
- Assessing ROI via revenue-to-median house price ratios (Queenstown: NZD 1.85M, Christchurch: NZD 0.7M).
- Visualizing trends to highlight seasonal and regional differences.

**Data Source**: AirROI API ([documentation](https://www.airroi.com/api/documentation/#tag/Listings)), stored in `nz_airbnb_all_metrics.csv`.

**Tools**: Python, pandas, matplotlib, requests.

## 🎯 Key Findings

- **Queenstown**:
  - Peaks in summer (Dec–Feb, e.g., NZD 13,392 revenue, 68% occupancy in January 2025) and winter (e.g., NZD 11,976 revenue in August 2024).
  - Revenue-to-price ratio (~0.0072 in January 2025) and high ADR (NZD 648.2) reflect strong ROI potential for short-term rentals.
  - 200–300 more active listings than Christchurch (e.g., 2,613 vs. 2,466 in January 2025).
- **Christchurch**:
  - Stable metrics (e.g., NZD 4,129 revenue, 60% occupancy, NZD 222.9 ADR in January 2025).
  - Lower revenue-to-price ratio (~0.0059) but consistent returns, ideal for long-term rentals.
- **Investment Insights**:
  - Queenstown suits high-yield, seasonal rentals but requires significant investment (NZD 1.85M).
  - Christchurch offers steady, lower-risk income (NZD 0.7M median price).

![Revenue-to-Price Ratio Plot](revenue_ratio.png)
*Line plot comparing revenue-to-median house price ratios for Queenstown and Christchurch (Aug 2024–Jul 2025).*

## 🚀 Getting Started

### Prerequisites
- **Python 3.8+**
- **Packages**: Install via `pip install -r requirements.txt`:
  - `requests`
  - `pandas`
  - `matplotlib`
- **AirROI API Key**: Set as an environment variable:
  ```bash
  export AIRROI_API_KEY='your-api-key'
