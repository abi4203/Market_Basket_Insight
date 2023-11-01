# Market_Basket_Insights README
Market Basket Insight is a data mining technique used by retail businesses to uncover valuable insights from customer transaction data. This GitHub repository houses a comprehensive project on Market Basket Analysis, focusing on understanding customer purchasing behavior and identifying cross-selling opportunities to optimize business strategies.

## Libraries Used
- numpy
- pandas
- matplotlib
- seaborn
- mlxtend
- plotly

## Data Source
The dataset is sourced from the "Assignment-1_Data.xlsx" file. It includes the following columns:
- BillNo
- Itemname
- Quantity
- Date
- Price
- CustomerID
- Country

## Data Preprocessing
1. The dataset was read from the Excel file with special handling for missing values marked as "?", "??", "???", "#", "##", "###", and "####".
2. Basic data trimming was applied to remove entries with missing or zero values in specific columns.
3. Outliers in the 'Quantity' and 'Price' columns were identified and capped.
4. Missing 'CustomerID' values were filled with dummy IDs.
5. Data types were converted for specific columns, and new columns were created based on date and time attributes.
6. A 'CountryID' column was created by categorizing countries.
7. The range of 'CustomerID' values was adjusted.

## Association Rule Mining
1. The item names from the transactions were extracted and one-hot encoded.
2. Frequent itemsets were mined using the Apriori algorithm.
3. Association rules were derived based on confidence and support thresholds.

## Visualization
1. The analysis was visualized using various plots.
2. A scatter plot showed the relationship between support, confidence, and lift.
3. Interactive visualizations were created with Plotly, including scatter plots and a sunburst chart for association rules.

## Usage
- To reproduce this analysis, ensure that you have the required libraries installed.
- Run the provided code in your preferred Python environment.

## Files
- `Assignment-1_Data.xlsx`: The dataset.
- `data_analysis.ipynb`: The Jupyter Notebook with the analysis code.
