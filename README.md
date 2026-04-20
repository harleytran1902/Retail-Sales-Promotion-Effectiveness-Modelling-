# Retail Sales & Promotion Effectiveness Modelling     
#### Python • R • Regression Modelling • Panel Data Analysis

## 1. Project Summary
- Retail brands often rely on heavy discounting to drive sales, but this can erode margins and create inconsistent performance across retailers.
- This project analyses pricing and promotion effectiveness to identify which strategies truly drive sales and how they should be optimised across different retail chains.

- This project explores how pricing and promotional activities influence product sales using multi-brand retail data collected across several supermarket chains over multiple years.
- The objective is to understand which marketing instruments are most effective, how sales respond to price changes, and whether promotional performance differs across retailers.
- Instead of focusing only on descriptive statistics, the project applies regression modeling and panel data techniques to measure the impact of marketing actions on sales and to provide data-driven recommendations for brand management.

## 2. Problem Statement
- Retail sales are affected by multiple factors, including price, discounts, in-store promotions, advertising, and store characteristics. However, the effectiveness of these factors is rarely constant across different retailers or time periods.

- The **main questions** addressed in this project are:
  - How sensitive are sales to price and discounts?
  - Which promotional activities generate the strongest sales response?
  - Do marketing effects differ across retail chains?
  - Do market conditions change the relationship between price, promotion, and sales?
  - Understanding these relationships is important for designing effective pricing and promotion strategies.

## 3. Data
- The analysis uses weekly retail data containing sales, prices, and promotion indicators for several brands across multiple supermarket chains over a multi-year period.

- Before modeling, the dataset was explored to check for missing values, outliers, and inconsistencies. Price distributions, sales trends, and promotion frequencies were analyzed to understand brand positioning and seasonal patterns.

- To avoid biased results, the data was cleaned and transformed before building the models, including removing invalid values, checking logical inconsistencies, and creating new variables to better represent discount intensity and promotion types.

<img width="676" alt="image" src="https://github.com/harleytran1902/Retail-Sales-Promotion-Effectiveness-Modelling-/raw/71bdcfaa6e61c0668e94bb4d855cde233b54e1ff/Weekly%20Sales%20Trends.jpeg">

<img width="676" alt="image" src="https://github.com/harleytran1902/Retail-Sales-Promotion-Effectiveness-Modelling-/raw/71bdcfaa6e61c0668e94bb4d855cde233b54e1ff/Promotion%20Activities.jpeg">


## 4. Method
- To measure the impact of marketing activities on sales, a multiplicative regression model was developed.

- The model includes variables representing price, discount level, different promotion types, and store-level differences. Because sales performance varies across retailers, dummy variables and partially pooled models were used to capture chain-specific effects.

<img width="676" alt="image" src="https://github.com/harleytran1902/Retail-Sales-Promotion-Effectiveness-Modelling-/raw/71bdcfaa6e61c0668e94bb4d855cde233b54e1ff/Model%201.jpeg">

- Several model specifications were tested to balance accuracy and interpretability. Log-transformation was applied to stabilize variance and allow elasticity interpretation of coefficients.

<img width="676" alt="image" src="https://github.com/harleytran1902/Retail-Sales-Promotion-Effectiveness-Modelling-/raw/71bdcfaa6e61c0668e94bb4d855cde233b54e1ff/Model%20Comparison.jpeg">

- To further account for differences between retailers, mixed-effects models were considered, allowing promotion effects to vary across chains. Model comparison was performed using goodness-of-fit criteria to select the most appropriate specification.

- Finally, structural changes over time were evaluated by testing whether the relationship between variables remained stable, which helps determine whether external market conditions altered consumer behavior.

## 5. Results
- The results show that sales are highly sensitive to price, with higher prices leading to a noticeable decline in demand. Discounts have a strong positive effect, indicating that temporary price reductions are one of the main drivers of sales.

- Promotional activities also influence sales, but their effectiveness depends on the type of promotion. Promotions that combine multiple marketing actions, such as increasing visibility together with advertising, have the strongest positive effect, while some promotion types are less effective when used alone.

- Sales performance also differs across retail chains, suggesting that store characteristics, customer base, and pricing strategies play an important role. Allowing promotion effects to vary across chains improves the model and provides a more realistic representation of the market.

- The analysis also indicates that relationships between price, promotion, and sales may change over time, meaning that models should be updated when market conditions shift.

## 6. Conclusion
- This project shows how statistical modeling can be used to understand the impact of marketing decisions on sales performance. By combining data exploration, regression analysis, and panel data methods, it is possible to identify which promotional strategies are most effective and how they should be adapted across different retailers.

- The results highlight the importance of considering both price sensitivity and store heterogeneity when designing marketing strategies, as well as the need to account for structural changes in the market over time.

**Key Note:**
- Pricing and promotion decisions should be tailored by retailer rather than applied uniformly.
- Discount-driven strategies can boost short-term sales but must be balanced against profitability.
- Data-driven pricing strategies can significantly improve both sales performance and marketing efficiency.


## 7. Business Recommendations
- Avoid excessive discounting as a primary growth strategy → focus on targeted promotions.
- Use combined promotion strategies (display + advertising) for maximum effectiveness.
- Adjust pricing and promotion strategies by retailer, as effectiveness varies significantly across chains.
- Continuously monitor price elasticity to optimise pricing decisions.




