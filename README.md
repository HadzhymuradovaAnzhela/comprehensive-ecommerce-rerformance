# Global E-commerce Revenue Analysis: Statistical Dependencies and Interactive Visualization
> Created with Google Colab, BigQuery and Tableau.  

This [project](comprehensive_ecommerce_performance_analysis.ipynb) focuses on identifying the primary drivers of financial performance for a global e-commerce platform. The analysis dives into revenue distribution across geographic regions, product categories, and acquisition channels. By utilizing the google.cloud.bigquery library for seamless data ingestion from BigQuery (SQL), using Python for performing in-depth statistical analysis, and developing an interactive dashboard in Tableau.  

**SQL Data Integration:**  
Merging tables (Full Outer and Left Joins)  

**Libraries Python:**  
* Cloud and Auth: google-cloud-bigquery, google.colab.auth
* Data Manipulation: pandas, numpy
* Statistical Analysis: scipy.stats (Pearson, Spearman, ANOVA, Mann-Whitney U, Kruskal-Wallis, Kendall), statsmodels
* Visualization: matplotlib, seaborn
  
**Tableau Visualization:**  
* Functional Analytics -  implemented revenue aggregations and advanced table calculations (WINDOW_MAX) to track peak performance.
* Visual Toolkit -  utilized Bar, Box, Line, Scatter, Bubble Chart, and Treemaps to represent result.
* User Experience - developed an interactive dashboard with seamless navigation and filters for data exploration.  

**Project Steps:**  
1. Data Import and Integration - imported 350k+ records from BigQuery using the google-cloud-bigquery library, executing SQL queries directly within Python for seamless data merging.  
2. Key Performance Metrics - identified top-performing countries, regions, categories, and channels through multi-level grouping, filtering, and sorting.
3. Revenue Segmentation Analysis - conducted an study of revenue distribution, quantifying the percentage impact of specific devices, acquisition channels, and operating systems etc.
4. User Engagement Profiling - analyzed user verification and subscription rates, compared revenue between guest and registered accounts, and identified geographical hotspots for account creation.
5. Sales Dynamics Analysis - evaluated overall sales trends and seasonality, comparing performance fluctuations across different regions, channels, and device types.
6. Cross-Dimensional Analysis - utilized pivot tables to examine the relationship between session volume and revenue across devices and channels, and analyzed average order value for subscribers vs. non-subscribers within top-performing categories.
7. Correlation Analysis - conducted a series of independent statistical studies to identify revenue drivers, investigating dependencies between Session Volume and Revenue, Regional Interdependence, Inter-Channel and Cross-Category relationships, as well as Registered vs. Guest purchase patterns. Each correlation was quantified using Pearson, Spearman, and Kendall coefficients and validated through p-value calculations to confirm statistical significance and reliability.
8. Comparative Analysis of Segmented Performance Metrics - performed rigorous hypothesis testing to validate differences across segments. This included using the Mann-Whitney U test to assess revenue significance by subscription status after analyzing variable distributions. For multi-group comparisons, such as traffic channel volume, ANOVA and Kruskal-Wallis tests were applied. Additionally, a Z-test for proportions was utilized to compare regional organic traffic shares and conversion rates.
9. Key Insights and Recommendations.
10. Interactive Dashboard -  developed a 2-page Tableau dashboard to visualize analytical findings. The first page focuses on high-level business metrics and sales dynamics, while the second page is dedicated to Revenue Drivers.

## Key Business Insights:
🌍 **Regional Dominance**  
The United States is the undisputed leader in both order volume and revenue, acting as the primary engine for global growth.  
🚀 **Acquisition Leaders**    
Organic Search is the most efficient channel, responsible for 35.8% of total income, followed by Paid Search and Direct traffic.  
🛋️ **Product Mix Strategy**  
A clear split exists between volume and value: Bookcases lead in sales quantity, but Sofas and Chairs generate the highest net revenue due to premium pricing.  
💻 **Technical Infrastructure**    
Desktop users contribute 59% of total revenue. The highest revenue volume is driven by the combination of Chrome, Safari (Desktop) and iPhone (Mobile) users.  
📧 **Subscription Impact**  
User loyalty is a key driver: 83.3% of revenue from registered users comes from Subscribers, proving the high financial efficiency of marketing communications.  
📈 **Cross-Selling Opportunities**  
Strong correlation between Seating and Storage categories suggests customers often buy them together, creating a clear basis for product bundling.  
📅 **Seasonal Peaks**   
Highest revenue spikes occur in early November and early January, with global trends highly synchronized across the Americas, Asia, and Europe.  

## Strategic Recommendations:  
🎯**Strategic Channel Development**  
Organic Search should remain the top priority as it is the primary source of user sessions (35.8%). Data shows a near-perfect correlation (Spearman 0.86) between total traffic volume and revenue growth. Unlike Organic or Direct traffic, Social Media channels demonstrate a different engagement dynamic. A separate, specialized marketing strategy is required for this segment to optimize its unique conversion paths and audience behavior.  
👥 **Customer Retention and Subscription**  
Data shows that 83.3% of total revenue is generated by registered subscribers. The company must implement a dedicated strategy (loyalty programs, welcome discounts, personalized email campaigns) to convert "guest" buyers into this high-value registered segment.  
🔄 **Cross-Selling Optimization**  
Increase Average Order Value by leveraging identified category dependencies. Specifically, customers purchasing seating solutions (Chairs and Sofas) should be targeted with recommendations for storage units (Bookcases), as these categories show strong purchasing synchronization.  
🌍 **Global Scaling Strategy**   
As conversion efficiency and organic traffic shares are statistically identical across the Americas and Europe, marketing resources should be allocated based on total traffic potential rather than regional funnel optimization.  

## [Interactive Dashboards (Tableau)](https://public.tableau.com/app/profile/angela.krupa/viz/GlobalEcommercePerformance/KeyInsights)
### Key Insights

<img width="1399" height="1000" alt="image" src="https://github.com/user-attachments/assets/799b4cbd-e953-4223-9248-cbb146a485e9" />


### Drivers   

<img width="1398" height="999" alt="image" src="https://github.com/user-attachments/assets/0b388e9a-951b-4a88-be99-86c942126cf5" />









