# sql-data-warehouse-project
# **Build Data Warehouse for Analytics and Business Insights**

This project uses **Microsoft SQL Server** to build a **Data Warehouse** from scratch, integrating data from **CRM and ERP sources**. The **ETL process** extracts raw data, performs **data cleansing and transformation**, and loads **structured data** into a star schema for business analytics.

---

## **Data Architecture**  
The data architecture follows the **Medallion Architecture** with **Bronze, Silver, and Gold layers**:  
<img width="1544" height="912" alt="data_architecture" src="https://github.com/user-attachments/assets/7beb8b08-0a3c-4e50-a05b-746b36b39979" />



1. **Bronze Layer**: Stores raw data **as-is** from the CRM and ERP sources. Data is ingested into SQL Server using **CSV files**.  
2. **Silver Layer**: Processes **data cleansing, standardization, and normalization** to enhance data quality and consistency.  
3. **Gold Layer**: Stores **business-ready** data, structured into a **star schema** for analytics and reporting.

---

## **Data Flow**  

<img width="1094" height="671" alt="data_flow" src="https://github.com/user-attachments/assets/d47c38f9-43ff-47ad-b7be-028c63ad4225" />

The data flow starts with **source systems (CRM & ERP)**, where raw data is collected and stored in the **Bronze Layer**. Next, in the **Silver Layer**, the data undergoes **cleansing, standardization, and integration** to remove inconsistencies. Finally, in the **Gold Layer**, transformed data is **modeled** into fact and dimension tables, making it **ready for business intelligence and reporting**.

### **Key Steps in the Data Flow:**  
1. **Extract**: Data is pulled from CRM and ERP in **CSV format**.  
2. **Transform**: The data undergoes **deduplication, formatting, and standardization**.  
3. **Load**: The cleaned data is stored in **fact and dimension tables** for efficient querying.  

---
