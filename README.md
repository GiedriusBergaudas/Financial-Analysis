# Retail Companies 2024 Financial Analysis

## Project Goal

This **project compares the 2024 financial performance of three major retail companies** with following market values:

- **Walmart ~$782 B**
- **Costco ~$413 B**
- **Target ~$48.2 B**

These companies are among the biggest in retail. The goal is to see which one had the strongest financial health in 2024 using key financial ratios.

## Tools Used

- Python  
- yfinance library  
- Pandas  
- Jupyter Notebook
- Seaborn
- Matplotlib

## Methodology

Using the `yfinance` Python library, I downloaded financial data for all three companies directly from Yahoo Finance. The data includes:

- **Income statements** 
- **Balance sheets**  
- **Cash flow reports**

Based on this data, I calculated seven important financial ratios to evaluate profitability, liquidity, efficiency, and debt.

Financial Ratios Used:

- **ROI**              
- **Gross Margin**   
- **Return on Sales**  
- **Current Ratio**    
- **Quick Ratio**     
- **Asset Turnover**   
- **Debt-to-Equity**   


## Scoring System

To compare the companies fairly, I built a scoring model:

1. Each ratio was scaled from 0 to 100 based on typical retail benchmarks.  
2. Each ratio was given a weight depending on its importance for retail companies.


| Metric          | Weight |                                              |
|-----------------|--------|-----------------------------------------------|
| ROI             | 30%    |    It is the most important because good returns are crucial for growth.          |
| Gross Margin    | 25%    |    Since retail depends a lot on controlling costs of goods sold, this ratio is very important.  |
| Return on Sales | 10%    |Shows how efficiently the company turns sales into profit.            |
| Current Ratio   | 10%    | Measures short term financial health and liquidity.        |
| Quick Ratio     | 5%     | A stricter liquidity test than the Current Ratio, but slightly less critical, so it has a smaller weight.                 |
| Asset Turnover  | 10%    | Shows how well the company uses its assets to generate sales, important for retail low margin environment.             |
| Debt-to-Equity  | 5%     | Retail companies usually carry moderate debt, so it has the lowest weight.         |

The final score is out of 100, where higher means better overall financial health.


## Results

| Company    | ROI (%) | Gross Margin (%) | ROS (%) | Current Ratio | Quick Ratio | Asset Turnover | Debt-to-Equity |
|------------|---------|------------------|---------|---------------|-------------|----------------|----------------|
| Walmart    | 18.50   | 24.38            | 3.78    | 0.83          | 0.24        | 2.57           | 1.93           |
| Target     | 30.81   | 27.54            | 5.40    | 0.91          | 0.29        | 1.94           | 3.12           |
| Costco     | 31.19   | 12.61            | 3.89    | 0.97          | 0.44        | 3.64           | 1.96           |

### Final Scores

- **Target: 70**  
- **Walmart: 62**  
- **Costco: 56**  

## Conclusion

**Target scored highest overall**, largely due to strong return and margin numbers. **Walmart** shows solid financials but scores lower mainly due to margins. **Costco** has excellent asset efficiency but lower margins impact its overall score.

Based on this analysis, **Target currently shows the strongest financial position** among these retailers.


