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
1. The Excel file containing the dataset was read, with special attention paid to any missing values indicated by the symbols "?", "??", "???", "#", "##", "###", and "####".
2. Simple data trimming was used to exclude items from particular columns that had zero or missing values.
3. 'Quantity' and 'Price' columns had outliers that were detected and capped.
4. Dummy IDs were used to fill in the missing 'CustomerID' entries.
5. In order to generate new columns based on date and time properties, certain columns' data types have to be modified.
6. The countries were categorized to produce a column called 'CountryID'.
7. A modification was made to the CustomerID's value range.

## Association Rule Mining
1. One-hot encoding was performed after extracting the item names from the transactions.
2. Using the Apriori technique, frequent itemsets were extracted.
3. Confidence and support thresholds were used to develop association rules.

## Visualization
1. A variety of graphs were used to visualize the analysis.
2. The relation between lift, confidence, and support was displayed using a scatter plot.
3. Using Plotly, interactive visualizations for association rules were produced, which included scatter plots and a sunburst chart.

## Usage
- Make sure you have the necessary libraries installed in order to replicate this analysis.
- Use the Python environment of your choice to run the provided code.


## Files
- `Assignment-1_Data.xlsx`: The dataset.
- `data_analysis.ipynb`: The Jupyter Notebook with the analysis code.
