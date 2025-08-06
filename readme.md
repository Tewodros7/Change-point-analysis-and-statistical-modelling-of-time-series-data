# Change Point Analysis of Brent Crude Oil Prices

## Project Overview

This project explores the impact of significant geopolitical and economic events on Brent crude oil prices throughout history. By employing Bayesian Change Point Detection methods using PyMC3, the aim is to uncover structural changes in oil price trends and link these changes to global occurrences such as conflicts, policy changes, and pandemics.

## Project Goals

- Identify statistically significant change points in Brent oil pricing.
- Relate these change points to documented historical events.
- Measure the extent and direction of price shifts.
- Present findings through reports and interactive dashboards.

## Dataset Information

- **Source:** Daily Brent crude oil prices from May 1987 to September 2022.
- **Fields:**
  - **Date:** Formatted as Day-Month-Year
  - **Price:** USD per barrel

An accompanying CSV file contains information on 11 major global events along with their respective dates for analysis.

## Directory Structure


.
├── data/
│   ├── brent_prices.csv
│   └── oilmarketevents.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02bayesianchangepoint_model.ipynb
├── app/
│   ├── dashboard.py
│   └── templates/
├── requirements.txt
├── README.md

## Technologies Used

* Python 3
* PyMC3 (for Bayesian modeling)
* pandas, matplotlib, seaborn (for EDA and visualizations)
* Flask (for the backend of the dashboard)
* React (frontend development, planned)

## Instructions for Use

1. Clone the repository.
2. Install the required dependencies:

   
bash
   pip install -r requirements.txt
   

3. Launch Jupyter notebooks to analyze the data and build models:

   
bash
   jupyter notebook
   

4. To run the dashboard (once implemented):

   
bash
   python app/dashboard.py
   


