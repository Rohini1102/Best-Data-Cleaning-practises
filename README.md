# Best-Data-Cleaning-practises
1. Understand the Data Context :
Before starting, review the data dictionary or metadata if available. Understanding the data's source, variables, and purpose helps identify what values make sense and flag any anomalies early on.

2. Remove Duplicates :
Duplicate entries can skew analysis results. Start by identifying unique identifiers (e.g., IDs) and checking for redundant rows. In cases where multiple similar entries are needed (e.g., different transactions by the same customer), set clear criteria for what constitutes a true duplicate.

3. Handle Missing Values :
Assess the percentage and location of missing values. If only a small portion is missing, consider removing those rows. For larger gaps, use imputation methods (e.g., mean, median, or mode) or advanced techniques like predictive imputation. However, avoid filling missing values in a way that introduces bias.

4. Standardize Data Formats :
Uniformity is essential for data to be processed accurately. Ensure consistent date formats (e.g., YYYY-MM-DD), standardized text formats (e.g., lowercase for case-insensitive columns), and uniform measurement units (e.g., converting all heights to centimeters).

5. Filter Outliers and Anomalies :
Outliers can distort analysis, especially if they result from data entry errors or unusual events. Use statistical techniques (like z-scores or interquartile ranges) to detect outliers and determine if they should be removed, adjusted, or retained, depending on the context.

6. Validate Data Types :
Ensure each column has the correct data type (e.g., numeric for quantitative data, string for categorical data). Misclassifications can result in calculation errors or unintended behaviors during analysis.

7. Use Consistent Coding for Categorical Values :
Categorical data should have consistent, meaningful labels. For example, instead of both "Male" and "M" for gender, choose one format. Additionally, avoid ambiguous labels by creating a predefined list of acceptable values for each category.

8. Handle Zeroes Carefully :
Zeroes may indicate missing data, valid measurements, or errors. Review each instance to determine if a zero is contextually appropriate or if it requires correction.

9. Address Cross-Field Validation :
Some values depend on each other (e.g., if "age" is less than 18, "employment status" should not be "employed full-time"). Check for these logical relationships to catch inconsistencies that may not be immediately obvious.

10. Remove Irrelevant Data :
Analyze which features or rows are necessary for your analysis. Removing irrelevant data reduces noise, improves model performance, and simplifies data processing.

11. Automate Cleaning Where Possible :
For large datasets, manual cleaning is time-consuming. Use scripts, data cleaning libraries, or tools (like Pandas in Python or Excel functions) to automate repetitive cleaning steps.

12. Document Cleaning Steps :
Document every modification, including removed rows, imputations, and transformations. A record of changes makes the process transparent and allows others to understand and replicate your work.

13. Validate Final Dataset :
After cleaning, re-check data accuracy with summary statistics (mean, median, etc.) or visualization techniques (boxplots, histograms) to verify improvements and ensure data integrity before moving on to analysis.
