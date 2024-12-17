# Exploratory Data Analysis on Oil and Gas Prices

## Overview

This repository contains a comprehensive Exploratory Data Analysis (EDA) conducted on oil and gas pricing data, leveraging advanced analytical techniques and robust visualization tools. The aim is to explore historical trends, uncover insights into market dynamics, and set the foundation for predictive modeling.

The notebook, [EDA oil and Gas Prices](https://github.com/Asonja12/EDA-on-Oil-and-Gas-Prices-/blob/main/EDA%20oil%20and%20Gas%20Prices.ipynb), systematically investigates price volatility, correlations, and patterns over time. The insights derived have potential applications in energy trading, market research, and policy-making.

---

## Dataset Description

The dataset used for this analysis contains daily pricing data for oil and gas commodities, with features that include:

| **Column**       | **Description**                                                                 |
|-------------------|---------------------------------------------------------------------------------|
| **Symbol**        | Type of commodity (e.g., Brent Oil).                                            |
| **Date**          | The recorded date of the price (YYYY-MM-DD).                                   |
| **Open**          | Opening price of the commodity for the trading day.                            |
| **High**          | The highest price reached on a specific day.                                   |
| **Low**           | The lowest price reached on a specific day.                                    |
| **Close**         | Closing price of the commodity.                                                |
| **Volume**        | The total trading volume for the commodity on the respective day.              |
| **Currency**      | The currency in which the commodity is priced (e.g., USD).                     |

### Dataset Properties
- **Time Span**: Multiple years of historical data (spanning decades).  
- **Granularity**: Daily-level pricing and volume data.  
- **Potential Extensions**: Could integrate with macroeconomic datasets, geopolitical event timelines, or regional price breakdowns.  

---

## Analysis Breakdown

The EDA process is structured as follows:

### 1. **Data Preprocessing and Cleaning**
   - **Missing Values**: Checked for null values and inconsistencies. The dataset was found to be complete, with no missing data.  
   - **Data Types**: Ensured appropriate data types for time-series analysis. Dates were converted to `datetime` objects for easy indexing.  
   - **Outlier Detection**: Analyzed extreme values in price and volume columns using boxplots and statistical thresholds.  

### 2. **Descriptive Statistics**
   - Summary statistics (mean, median, standard deviation) were calculated for `Open`, `Close`, `High`, and `Low` prices.  
   - Volume distributions were plotted to understand market activity trends.  

### 3. **Trend and Seasonality Analysis**
   - **Time-Series Visualization**:  
     - Line charts for `Close` prices over time revealed historical trends and key events, such as the 2008 financial crisis and the 2020 oil price collapse.  
   - **Seasonality**:  
     - Monthly and yearly averages were computed to identify recurring patterns (e.g., price spikes during winter months due to heating demand).  

### 4. **Volatility Analysis**
   - **Daily Returns**: Calculated daily price changes to quantify market volatility.  
   - **Rolling Statistics**: Rolling means and standard deviations were computed to smooth trends and identify periods of heightened volatility.  

### 5. **Correlation Analysis**
   - **Pairwise Correlations**: Examined relationships between `Open`, `Close`, `High`, and `Low` prices.  
   - **Volume vs. Price**: Weak correlation observed, indicating that volume changes may not directly drive price movements.  

### 6. **Event-Driven Analysis**
   - Price movements were annotated with key global events to understand external impacts (e.g., the COVID-19 pandemic, geopolitical tensions).  

---

## Key Insights

### **Trends and Patterns**
- **Historical Trends**:  
  - Long-term growth interspersed with sharp price declines during crises.  
  - A steady rise in prices is observed post-crisis recovery periods.  

- **Seasonality**:  
  - Prices tend to rise in winter months, reflecting increased demand for heating oil.  
  - Volumes spike during volatile periods, indicating higher trading activity.  

### **Market Volatility**
- Oil prices experienced extreme volatility in 2008 and 2020, driven by economic uncertainty and global demand shocks.  
- Rolling standard deviation reveals clusters of high volatility, often aligning with global crises or geopolitical disruptions.  

### **Correlation Analysis**
- Strong positive correlation between `High` and `Close` prices, as expected in financial data.  
- Weak correlation between trading volume and daily price changes suggests external factors (e.g., news events) have greater influence on prices.  

### **Event Impacts**
- **2008 Financial Crisis**: Oil prices plummeted by over 60% during the global recession.  
- **COVID-19 Pandemic**: Negative prices briefly occurred due to storage challenges and demand collapse in 2020.  

---

## Technical Highlights

1. **Visualization**:  
   - Used line charts, heatmaps, and rolling windows to illustrate trends and correlations effectively.  
   - Included annotated visualizations for event-driven price movements.  

2. **Statistical Analysis**:  
   - Performed hypothesis testing to validate relationships between variables.  
   - Used z-scores to identify anomalies in price trends.  

3. **Time-Series Techniques**:  
   - Decomposed time-series data into trend, seasonal, and residual components for advanced analysis.  
   - Applied moving averages to smooth noisy data and highlight key patterns.  

4. **Annotations**:  
   - Key insights were enriched with annotations to explain price movements and outliers in the context of external events.  

---

## Repository Structure

```plaintext
|-- data/
|   |-- oil_and_gas.csv       # Dataset used for the analysis
|-- notebooks/
|   |-- EDA_oil_and_gas.ipynb # Main Jupyter Notebook containing the analysis
|-- visuals/
|   |-- trends.png            # Price trend over time
|   |-- correlations.png      # Heatmap of variable correlations
|-- README.md                 # This file
```

---

## How to Use

1. Clone the repository:  
   ```bash  
   git clone https://github.com/Asonja12/EDA-on-Oil-and-Gas-Prices-.git  
   cd EDA-on-Oil-and-Gas-Prices-  
   ```  

2. Install the required Python libraries:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. Open and run the notebook:  
   ```bash  
   jupyter notebook notebooks/EDA_oil_and_gas.ipynb  
   ```  

---

## Future Directions

- Integrate additional macroeconomic indicators such as inflation, GDP, and exchange rates to enrich the analysis.  
- Incorporate external datasets (e.g., geopolitical events, weather patterns) to contextualize price movements.  
- Develop machine learning models to predict future prices based on historical trends.  

---

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for new features or analyses, feel free to open an issue or submit a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---


