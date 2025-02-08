This Python script processes transaction data to calculate and analyze key metrics for online sales, focusing on Recency, Frequency, and Monetary Value—essential components of Customer Lifetime Value (CLV) analysis.

Key Functionalities:
Dataset Loading:

The script loads a dataset named Online_Sales.csv using pandas. This dataset likely contains customer transaction details, including transaction dates, customer IDs, and purchase prices.
Data Preprocessing:

Ensures that the Transaction_Date column is converted to a datetime format for accurate date-based calculations.
CLV Metric Calculation:

Recency: Measures the number of days since a customer's last transaction, using the most recent transaction date as the reference.
Frequency: Counts the number of unique transactions per customer.
Monetary Value: Sums the total transaction value (Avg_Price) for each customer.
Revenue: Represents the total monetary value for each customer.
Customer Segmentation:

Groups data by CustomerID to aggregate these metrics and reset the index for further analysis.
Sorting by CLV:

Customers are sorted by their calculated CLV to identify high-value customers.
Libraries Used:
pandas: For data manipulation and aggregation.
