**RFM Approach in E-Commerce**

**Datasouce path**:

https://www.kaggle.com/datasets/carrie1/ecommerce-data/data

**Context**:

Typically e-commerce datasets are proprietary and consequently hard to find among publicly available data. However, The UCI Machine Learning Repository has made this dataset containing actual transactions from 2010 and 2011. The dataset is maintained on their site, where it can be found by the title "Online Retail".

**Content**:

"This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers." There are around 540,000 transactions in the dataset.

**Approach**:

Data Study was conducted after importing the dataset. Duplicates were removed and fields were converted to appropriate datatype. 'TotalPrice' field was created and was calculated using the "Quantity' and 'UnitPrice' fileds. Few visualisations were created to study more about the data.

Significant fields for the RFM (Recency-Frequency-Monetary) approach were filtered out and null values were dropped. Grouping the customers based on CustomerID and aggregations done on the rest of the columns to know the Recency, Frequency and Monetary values. Quantile method was used to know the qunatiles in the RFM values and custom functions were used on the RFM values to compare it with the quantiles to segregate them. Consolidated RFM values were calculated and 'qcut' method was used to group the customers into 4 categories (Platinum, Diamond, Gold, Silver)

Visualisation was created to know the number of customers in each group. 

