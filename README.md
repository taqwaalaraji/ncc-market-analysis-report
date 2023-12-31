# Market Analysis Report for National Clothing Chain

## Overview

We are partnering with a national clothing chain that operates online. Recently, they've experienced a stagnation in sales and are keen on reviving their business by attracting lost customers back. To achieve this, they aim to implement a targeted marketing campaign, advertising specific products to specific customers in specific locations.

They've identified three key products for this campaign:

- Shirt: $25
- Sweater: $100
- Leather Bag: $1,000

The challenge lies in identifying who to target for each product. This is where your expertise is required. Your task is to conduct an in-depth analysis to determine the best product to advertise to each customer.

## Project Specifications

### Power Query
- The 'Product Inventory' table in the Customer List is successfully joined and split into six columns. All columns are labeled with correct formatting and do not produce any Power Query errors.
- The 'Purchase List' table is unpivoted, organized, and has a date column correctly formatted as a date. No Power Query errors are present for any of the columns or rows.

### DAX
- A DAX formula is used to define income categories, aggregating the different predicted customer incomes into buckets. This formula is used to generate a histogram, providing a reflection of the data's range, distribution, and shape. The histogram contains at least four columns.
- A DAX formula is created to define product recommendations. This formula determines which products are recommended to different income categories.

### Visualization & Analysis
- A linear regression formula is created to predict customer incomes based on sales and income. The formula 'y = mx + b' is used, with 'm' and 'b' replaced with actual values.
- A histogram is created to show the distribution and shape of predicted income by category. It's developed using a column chart and the previously created DAX formula.
- A scatter plot with trendline and correlation coefficient quick measure (displayed on a card) is utilized to perform a regression analysis of the relationship between average household income and average six-month sales by state.
- A heatmap is used to visualize household income distribution across the U.S.
- Table relationships are set up correctly to allow cross-filtering in visualizations. Specifically, histogram columns can update the heatmap, and the scatterplot can update both the histogram and the map.
- The findings are presented in a detailed written summary that includes the results, conclusions, and recommendations of the analysis. The document addresses all analysis questions, provides the formula for predicting customer incomes, explains scatterplot relationships with R-squared values, includes research findings on 1-2 additional variables, specifies visuals that contribute to the narrative, and presents recommendations based on the results of the statistical analysis.

## Final Report

This report presents our comprehensive analysis of the relationships between customer sales, income, ratings, product return rates, and provides strategic insights for enhancing our marketing approach.

### Key Findings
1. **Correlation between sales and income**: A strong correlation (R^2 = 0.78) was observed between sales and income, indicating that income increases are associated with increased sales. States such as Columbia, Maryland, and Massachusetts, which are among the top five highest-income states, demonstrate high sales figures.

2. **Correlation between customer ratings and product return rate**: A significant correlation (R^2 = 0.69) was found between customer ratings and product return rates. Products with higher ratings tend to have lower return rates, suggesting customer satisfaction with those products.

3. **Predicted customer incomes and sales**: A linear regression formula, X= b-Y/-m, was utilized to predict customer incomes and sales. Here, X is the average income, and Y is the average sales.

4. **Customer with the highest predicted income**: Our analysis identified Jon Little as the customer with the highest predicted income.

5. **Most advertised product**: Given lower return rates (indicating higher customer satisfaction), highly rated products such as the cotton sweater should be prioritized in our marketing campaigns.

### Data Visualization
Our analysis employed various data visualization methods:
- **Scatterplots** illustrated the relationship between sales and income.
- **Histograms** segmented predicted income into discrete categories.
- **Heat maps** identified states with higher average incomes.
Trend lines in scatterplots visibly demonstrated the direction and strength of correlations.

### Additional Variables
We considered geographical location (state) and customer demographics in our analysis. Despite high average incomes, certain states like New Jersey and Hawaii have underexploited sales potential. Similarly, specific demographic segments showed higher profitability.

### Recommendations
Based on our findings, we propose a marketing strategy that focuses on high-income states with untapped sales potential, particularly New Jersey and Hawaii. Targeted advertising campaigns could yield considerable returns in these regions.

Customer demographic data can further refine our marketing efforts, helping us to reach high-income customer segments more effectively. We particularly recommend focusing on customers with the highest predicted income, like Jon Little.

### Data Processing
The 'Product Inventory' table from the Customer List was split into six columns. The 'Purchase List' table was unpivoted, organized, and featured a correctly formatted date column. Customer incomes were aggregated into a histogram to show the distribution and shape of predicted income by category. 

### Product Recommendations
Product recommendations were defined for different income categories. We used linear regression (formula: X= b-Y/-m) to predict customer incomes, with a specific example where Y= 219.91, M =0.01, B= -722.14 yielding a predicted income X= 94,205.

### Regression Analysis
A scatter plot with a trendline and the correlation coefficient was used to analyze the relationship between the average income by state and the average six-month sales by state. The heatmap visualized household income distribution across the US. 

### Cross-filter
Cross-filter functionality was implemented where histogram columns can update the heatmap, and the scatterplot can update both the histogram and the map.


## Final Report Screenshots

### The Project Model
![The Project Model](images/screenshots/project-model.png)

### Final Report
![Final Report](images/screenshots/final-report.png)
