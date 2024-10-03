# Exploratory-Data-Analysis-EDA-of-Global-Layoffs-Using-SQL
The project aims to conduct an Exploratory Data Analysis (EDA) on global layoff data to uncover trends, patterns, and insights such as the largest layoffs by companies, locations, industries, and countries over time. The goal is to understand the magnitude and distribution of layoffs across different factors.

### Key Features:
1. **Basic Exploration**:
   - **Finding Maximum and Minimum Layoffs**: Simple queries to explore the maximum and minimum layoffs (`total_laid_off`) and `percentage_laid_off` to understand the scale of layoffs.
   - **Identifying Companies with 100% Layoffs**: Companies that laid off all of their employees (100% layoffs) are identified, with many of them being startups that went out of business.

2. **Ranking by Layoff Magnitude**:
   - **Largest Layoffs by Company**: Queries are used to identify which companies had the largest single-day layoffs and which companies had the highest total layoffs.
   - **Layoffs by Location and Country**: Grouping by location and country to find areas most impacted by layoffs.
   - **Layoffs by Industry**: Understanding the layoffs distributed by industry, revealing which sectors are most affected.
   - **Layoffs by Funding Stage**: Grouping and ranking layoffs by funding stage (e.g., Series A, B, etc.).

3. **Year-over-Year Layoff Trends**:
   - **Layoff Trends by Year**: Year-over-year trends are identified, showing how layoffs have evolved annually.
   - **Top 3 Companies by Layoffs per Year**: Using a combination of CTEs and `DENSE_RANK()`, the project identifies the top three companies with the most layoffs each year.

4. **Rolling Layoff Totals**:
   - **Rolling Total Layoffs Per Month**: A rolling total of layoffs per month is calculated, providing insight into how layoffs accumulate over time.
   - **CTE-Based Analysis**: A CTE is used to generate rolling totals, which can be queried for more flexible insights.

### Technologies Used:
- **SQL**: Various SQL techniques are employed for the EDA, including:
  - **Window Functions** (`DENSE_RANK()`, `ROW_NUMBER()`).
  - **Common Table Expressions (CTEs)** for subqueries and complex query chains.
  - **Aggregate Functions**: `SUM()`, `MAX()`, `MIN()`.
  - **Date Functions**: `YEAR()`, `SUBSTRING()` for date-based grouping.
  
- **Analytical SQL Concepts**: Grouping, ranking, rolling totals, and temporal data analysis are key components of this project.

### Result/Impact:
- **Key Insights on Layoffs**: The EDA uncovered valuable insights, such as companies and industries most impacted by layoffs, the locations with the highest layoffs, and trends in layoffs over time.
- **Identification of Outliers**: Outliers, such as companies laying off 100% of their employees, were identified, highlighting sectors under stress during specific periods.
- **Temporal Analysis**: Rolling totals of layoffs provided a view of how layoffs accumulate and when spikes occur, allowing for better understanding of economic impacts.

The project provided comprehensive layoff insights, making it valuable for business leaders, policymakers, and analysts studying economic trends.
