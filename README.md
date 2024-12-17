# Exploratory Data Analysis on Oil and Gas Prices

## Overview
This repository contains an Exploratory Data Analysis (EDA) of oil and gas prices over time. The dataset includes daily price and volume information for oil and gas commodities such as Brent Oil, spanning from the year 2000 onward. The purpose of this analysis is to uncover patterns, trends, and insights that can inform trading strategies, market predictions, and investment decisions.

## Dataset Description
The dataset used in this analysis consists of the following columns:

| Column   | Description                                                                 |
|----------|-----------------------------------------------------------------------------|
| Symbol   | The type of commodity (e.g., Brent Oil).                                    |
| Date     | The date of the record (YYYY-MM-DD format).                                 |
| Open     | The opening price of the commodity.                                        |
| High     | The highest price of the commodity for the day.                            |
| Low      | The lowest price of the commodity for the day.                             |
| Close    | The closing price of the commodity.                                        |
| Volume   | The trade volume for the commodity on the respective day.                  |
| Currency | The currency in which the commodity prices are quoted (e.g., USD).         |

### Key Features
- **Time Range**: Data spans over multiple decades starting from the year 2000.
- **Comprehensive Metrics**: Includes open, high, low, and close prices, along with trade volume.
- **Multi-commodity Support**: While the sample indicates "Brent Oil," the dataset could potentially support additional commodities.

## Analysis Goals
1. **Understand Historical Trends**: Analyze how oil and gas prices have fluctuated over time.
2. **Detect Seasonal Patterns**: Investigate recurring trends based on months or years.
3. **Examine Volatility**: Explore periods of high and low volatility in the market.
4. **Identify Correlations**: Analyze relationships between trading volume and price movements.
5. **Predictive Modeling Foundation**: Provide insights for future forecasting models.

## Key Insights from the Analysis
### Present in the Dataset:
1. **Historical Price Trends**: Prices have varied significantly over the decades, influenced by global events such as economic crises, geopolitical tensions, and technological advancements in energy.
2. **Volatility**: Notable periods of high price volatility align with major market events, e.g., the 2008 financial crisis or the 2020 pandemic.
3. **Volume-Price Relationship**: A preliminary analysis suggests a weak correlation between trade volume and price movement, which varies across different timeframes.
4. **Seasonal Fluctuations**: Early analysis indicates potential seasonal trends, with certain months showing consistent price spikes or drops.

### Absent but Can Be Gleaned:
1. **Impact of External Events**: The dataset does not explicitly capture external factors such as policy changes, wars, or natural disasters, but combining it with external data could provide deeper insights.
2. **Regional Pricing Differences**: The dataset lacks regional breakdowns for commodities, which could highlight disparities in pricing dynamics across global markets.
3. **Commodity Comparisons**: If additional commodities are added, cross-commodity comparisons could reveal substitution effects or complementary trends.
4. **Inflation-Adjusted Prices**: The prices are nominal and not adjusted for inflation, which is crucial for long-term trend analysis.

## Repository Structure
```
- data/
    - oil_and_gas.csv       # The dataset used in the analysis
- notebooks/
    - eda.ipynb            # Jupyter Notebook containing the analysis
- visuals/
    - trends.png           # Line graph of historical price trends
    - volatility.png       # Volatility heatmap over the years
- README.md                # This ReadMe file
```

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo-name.git
   ```
2. Install the necessary Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook for detailed analysis:
   ```bash
   jupyter notebook notebooks/eda.ipynb
   ```
4. Explore the `visuals/` folder for key graphs and figures generated during the analysis.

## Dependencies
- Python 3.8+
- pandas
- matplotlib
- seaborn
- numpy
- Jupyter Notebook

## Future Work
- Integrate additional datasets, such as geopolitical events and inflation indices, for enriched analysis.
- Develop predictive models using machine learning techniques.
- Add more visualizations to highlight patterns and anomalies.
- Explore regional breakdowns and their impact on global prices.

## Contributing
Contributions are welcome! If you have suggestions or additional datasets that can enhance this analysis, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

Feel free to reach out for any questions or clarifications. Happy analyzing!

