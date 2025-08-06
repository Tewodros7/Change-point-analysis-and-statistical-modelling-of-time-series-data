# Brent Oil Price Analysis Framework

## 1. Data Analysis Process

1. **Data Gathering & Preparation**
   - Import Brent oil prices from data/raw/BrentOilPrices.csv.
   - Clean and preprocess the dataset (address missing values, confirm correct data types).
   
2. **Exploratory Data Analysis (EDA)**
   - Visualize the time series to observe trends, seasonality, and volatility.
   - Assess stationarity (e.g., using the ADF test).
   - Identify significant time periods.
   
3. **Compilation of Event Data**
   - Gather major oil market events from data/MajorOilMarketEvents.csv.
   - Synchronize these events with the timeline of Brent oil prices.
   
4. **Change Point Detection**
   - Utilize change point algorithms to identify structural shifts.
   - Compare identified change points with known events.
   
5. **Modeling**
   - Fit statistical models to the segments between change points.
   - Assess model performance and interpret the results.
   
6. **Reporting & Communication**
   - Summarize findings using visuals and concise narratives.
   - Prepare deliverables for stakeholders (reports, presentations, dashboards).

## 2. Assumptions and Constraints

### Assumptions:
- The Brent oil price data is accurate and representative of the market.
- Event dates are approximate and may not align precisely with price fluctuations.
- Change point models identify statistical breaks rather than causal relationships.

### Limitations:
- Statistical correlation does not equate to causation.
- External factors not included in the event data may affect prices.
- Change point detection can be influenced by noise and choice of parameters.

## 3. Communication Methods
- Written reports (PDF, Word)
- Interactive dashboards (Jupyter, web applications)
- Presentations (PowerPoint, Google Slides)
- Visual representations (charts, timelines)

## 4. Understanding the Model and Data
- **References:** Review essential literature on change point detection and time series analysis.
- **Properties of Time Series:**
  - Examine trends and stationarity before modeling.
  - Stationarity will guide model selection (e.g., ARIMA vs. regime-switching models).
- **Change Point Models:**
  - **Objective:** Identify structural changes within time series data.
  - **Outputs:** Dates of changes, parameter variations, segment statistics.
  - **Limitations:** May identify false breaks; not all detected breaks are significant.
