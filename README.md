Forecasting Net Prophet
Project Overview
This project analyzes MercadoLibre's Google search traffic data to determine if search patterns can predict stock trading success. As a growth analyst at MercadoLibre (Latin America's most popular e-commerce site with over 200 million users), the goal is to identify clever ways to analyze financial and user data to help the company grow.
Background
MercadoLibre is the leading e-commerce platform in Latin America. This analysis explores whether the ability to predict search traffic can translate into successful stock trading strategies by examining the relationship between Google search trends and stock price movements.
Project Structure
The analysis is divided into four main steps:
Step 1: Find Unusual Patterns in Hourly Google Search Traffic

Analyzed search traffic during May 2020 when MercadoLibre released quarterly financial results
Key Finding: Search traffic increased by approximately 8.55% during the financial results release month compared to the median monthly traffic

Step 2: Mine the Search Traffic Data for Seasonality

Examined patterns by hour of day, day of week, and time of year
Key Findings:

Hourly patterns: Greatest popularity occurs around midnight (00:00) and 10:00 PM
Weekly patterns: Tuesday shows the highest search traffic
Seasonal patterns: Lowest search traffic occurs in mid-to-late October



Step 3: Relate the Search Traffic to Stock Price Patterns

Combined search data with stock price data for correlation analysis
Created lagged search trends, stock volatility, and hourly return metrics
Key Finding: Weak correlation between lagged search traffic and stock volatility (-0.149) or stock returns (0.018), indicating limited predictive power

Step 4: Create a Time Series Model with Prophet

Built a Prophet forecasting model to predict future search trends
Generated 80-day forecasts with confidence intervals
Key Finding: Near-term forecast shows a slight declining trend in search popularity

Technologies Used

Python: Primary programming language
Pandas: Data manipulation and analysis
Matplotlib: Data visualization
Prophet: Time series forecasting
Google Colab: Development environment

Key Insights

Financial Events Impact: Search traffic increases during significant financial announcements, suggesting public interest correlates with corporate events.
Predictable Patterns: Clear seasonal patterns exist in search behavior:

Daily peaks around midnight and evening hours
Weekly peaks on Tuesday
Annual lows in October


Limited Stock Prediction: While search trends show patterns, they have weak predictive power for short-term stock movements.
Marketing Implications: Understanding when users are most active can help optimize marketing campaigns and budget allocation for maximum ROI.

Business Applications
For Marketing Teams:

Optimal Timing: Schedule campaigns during peak hours (midnight and 10 PM) and peak days (Tuesday)
Budget Allocation: Increase marketing spend during high-traffic periods
Seasonal Planning: Prepare for lower engagement in October

For Financial Analysis:

Event Monitoring: Track search spikes around earnings releases as an indicator of public interest
Investor Relations: Understand that financial announcements generate measurable public attention

For Strategic Planning:

Trend Analysis: Use search patterns to gauge long-term brand interest
Market Sentiment: Monitor search trends as one component of overall market analysis

Files in This Repository

forecasting_net_prophet.ipynb: Complete Jupyter notebook with analysis and visualizations
README.md: This file providing project overview and insights

Data Sources

Google search trends data for MercadoLibre (hourly data from 2016-2020)
MercadoLibre stock price data (corresponding time period)
Data accessed via provided URLs in the assignment

Methodology

Data Collection: Retrieved hourly search trends and stock price data
Data Cleaning: Processed and aligned time series data
Pattern Analysis: Identified seasonal and temporal patterns
Correlation Analysis: Examined relationships between search trends and stock metrics
Forecasting: Applied Prophet model for future trend prediction
Interpretation: Analyzed results for business insights

Conclusions
While Google search traffic shows clear patterns and responds to financial events, it has limited utility as a standalone predictor for stock trading. However, search trend analysis provides valuable insights for marketing optimization, brand monitoring, and understanding customer engagement patterns. The predictable seasonal patterns identified can help MercadoLibre optimize their marketing strategies and improve customer acquisition timing.
Future Research Opportunities

Analyze correlation with longer-term stock performance
Incorporate additional external factors (economic indicators, competitor analysis)
Explore sentiment analysis of search query content
Examine regional search pattern variations across Latin American markets
Develop more sophisticated machine learning models combining multiple data sources

Author
Growth Analyst - MercadoLibre Data Science Team

This analysis was completed as part of a time series forecasting challenge using Prophet and real MercadoLibre data.
