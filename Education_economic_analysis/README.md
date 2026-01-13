1(Introduction)
Education is a fundamental driver of social and economic development. Understanding how economic conditions influence educational access and academic performance is crucial for policymaking, especially in conflict-affected countries.
This project investigates the relationship between economic indicators, such as GDP per capita and unemployment rate, and educational outcomes, focusing on three countries: Syria, France, and Germany. The goal is to highlight disparities, trends, and policy implications for improving access to education.
2️⃣(Data Overview)
Sources: Combined datasets from global economic and educational statistics (GDP per capita, unemployment rate, school enrollment, literacy rates).
Time Period: 1999–2022 for education data; 2010–2025 for economic data.
Countries: Syria (conflict-affected), France, Germany (European benchmarks).
Key Variables:
gdp_per_capita (GDP per capita in USD)
unemployment_rate (%)
school_enrol_secondary_pct (Secondary school enrollment %)
school_enrol_tertiary_pct (Tertiary education enrollment %)
Missing values were retained to avoid introducing bias, particularly for Syria where gaps are linked to conflict and structural instability.
3️⃣  (Methodology)
The analysis was conducted in Python (Google Colab) using:
Pandas: Data cleaning and preparation
Matplotlib & Seaborn: Visualization (heatmaps, scatter plots, boxplots)
Statsmodels: Linear regression analysis
Steps:
Data Cleaning: Renamed columns, converted numeric values, handled missing data by retaining gaps.
Exploratory Analysis: Summary statistics to understand distributions and differences among countries.
Correlation Analysis: Computed correlation matrix to examine linear relationships.
Regression Analysis: Linear regression between GDP per capita and tertiary education enrollment.
Country Comparison: Visualized disparities using boxplots.
4️⃣ (Results)
4.1 (Descriptive Analysis)
Secondary and tertiary enrollment rates are generally higher in France and Germany compared to Syria.
Syria shows significant gaps during conflict years (2011–2020).
GDP per capita and unemployment rate differ widely across countries, influencing access to higher education.
4.2 (Correlation Analysis)
Correlation Heatmap
GDP per capita positively correlates with tertiary education enrollment (strong correlation ~0.78).
Unemployment rate shows weak negative correlation with secondary and tertiary enrollment.
Interpretation: Higher economic prosperity is associated with higher participation in tertiary education, whereas economic instability limits opportunities.
4.3 (Regression Analysis)
OLS Regression Results:
Dependent Variable: Tertiary Education Enrollment (%)
Independent Variable: GDP per Capita (USD)
R-squared = 0.780 → 78% of variation in tertiary enrollment explained by GDP per capita.
Coefficient (GDP per capita) = 0.0007 → Increase of $1000 in GDP per capita corresponds to ~0.7% increase in tertiary enrollment.
P-value < 0.001 → Relationship is statistically significant.
Interpretation: Economic growth is strongly associated with increased access to higher education. Structural disparities are evident in conflict-affected countries like Syria.
Regression Scatter Plot with Trendline:
Shows clear positive trend between GDP per capita and tertiary enrollment.
4.4 (Country Comparison)
Boxplot Results:
France and Germany: High tertiary enrollment rates (50–80%)
Syria: Lower and more variable tertiary enrollment (20–50%)
The results highlight substantial gaps in educational access between European and conflict-affected countries.
5️⃣(Discussion & Conclusion)
Economic Influence:
Higher GDP per capita strongly predicts greater tertiary education enrollment.
Policy implication: Investment in economic stability can indirectly improve education outcomes.
Conflict Impact:
Syria shows missing data and lower enrollment due to prolonged conflict.
International support is crucial to mitigate educational disruptions.
Policy Recommendations:
Strengthen economic policies supporting households’ capacity to send children to school.
Targeted educational programs for conflict-affected regions.
Monitor enrollment trends regularly using integrated economic and educational datasets.
Limitations:
Missing data for Syria in certain years
Univariate regression; future studies could include multivariate factors (literacy, government expenditure, pupil-teacher ratio).
Overall, this project demonstrates a strong linkage between economic conditions and educational access, with implications for global development policy and scholarship considerations.
6️⃣ (Figures)
Correlation Heatmap → Shows relationships between GDP, unemployment, and enrollment.
Scatter Plot (GDP vs Tertiary Enrollment) → Positive trend clearly visible.
Boxplot by Region → Highlights disparity between Europe and conflict-affected Syria.
