## Elevation_Bike_Store_Dashboard

Interactive Power BI dashboard analyzing sales, returns, and trends for the Elevation Bike Store project.
Includes insights for different managerial roles, detailed return loss breakdowns, and product-level performance analysis.
All datasets are fictional but have been designed to reflect realistic business scenarios and data relationships.
---

## 📂 Project Files
- 📊 [Dashboard (.pbix)](Dashboard%20Elevation%20Bike%20Store.pbix)  
- 📜 [DAX Measures](DAX_Measures_Elevation_Bike_Store)  
- 📂 **Data Files:**
  - [Categories.csv](data/Categories.csv)  
  - [Customer_Types.csv](data/Customer%20Types.csv)  
  - [Customers.csv](data/Customers.csv)  
  - [Products.csv](data/Products.csv)  
  - [Returns.csv](data/Returns.csv)  
  - [Sales.csv](data/Sales.csv)  
  - [Staff.csv](data/Staff.csv)  
  - [Stocks.csv](data/Stocks.csv)  
  - [Stores.csv](data/Stores.csv)  
  - [Sub_Categories.csv](data/Sub%20Categories.csv)  

********************************************************************************************************************************************************************

## Executive Summary
----------------------

Over the past 2.5 years, Elevation Bike Store has faced €765,000 in return losses, with 75% of these losses concentrated in just five bike models—the majority being race bikes. Bicycles account for 96% of all return-related losses, and the UK market alone is responsible for 60% (€459,000) of total return value.

The customer base currently includes only individuals aged 46 and above, indicating a missed opportunity to attract younger buyers.
Key priorities are clear: address high-return models, focus on loss-heavy regions, and implement targeted marketing to engage a younger demographic.

*****************************************************************************************************************************************************************************************************************

## Data Modeling (ERD)
--------------------------
<img width="1110" height="537" alt="Screenshot 2025-08-21 072722" src="https://github.com/user-attachments/assets/02852055-e123-4db0-a6cb-c90ea09f9249" />

Table Relationships and Keys

BlankReturnProductIDs (ID) → Products (ID)

Customers (CustomerID) → Customer Types (ID)

Products (SubcategoryID) → Sub Categories (ID)

Returns (ProductReturned) → Products (ID)

Returns (ReturnedIn) → Stores (ID)

Sales (ProductSold) → Products (ID)

Sales (SoldBy) → Staff (StaffMemberID)

Sales (SoldIn) → Stores (ID)

Sales (SoldTo) → Customers (CustomerID)

Stocks (ProductID) → Products (ID)

Stocks (StoreID) → Stores (ID)

Sub Categories (CategoryID) → Categories (ID)

All relationships are many-to-one, enforcing referential integrity.

**************************************************************************************

## 📌 Key Insights

€765,000 in returns recorded over 2.5 years, with €571,000 (75%) of total return losses attributable to just five bike models.

Bicycles represent 96% of all return losses, with the UK market alone accounting for approximately €459,000 (60%) of total losses.

Among the most returned models, four out of five are race bikes, indicating a recurring issue concentrated in this product category.

A small subset of models is responsible for the majority of financial losses, emphasizing the need for focused interventions at the product level.




<img width="1290" height="731" alt="image" src="https://github.com/user-attachments/assets/f2dd9c12-20c7-4508-865a-42c67981bfc2" />

<img width="1293" height="732" alt="image" src="https://github.com/user-attachments/assets/21cc38d6-46e8-414e-87e2-156867653baa" />

<img width="1297" height="732" alt="image" src="https://github.com/user-attachments/assets/53e2a8c6-639e-4062-9902-94f8734a6cff" />

<img width="1297" height="732" alt="image" src="https://github.com/user-attachments/assets/17772d25-8ac8-40b9-a2ed-40c9ccd769b7" />

<img width="1297" height="732" alt="image" src="https://github.com/user-attachments/assets/dc242f2f-23ca-40ee-944f-e5c01403150f" />

<img width="1295" height="735" alt="image" src="https://github.com/user-attachments/assets/ca716fe5-df3e-439c-9231-c72d8e2473ca" />

************************************************************************************************************************************************

## Assumptions and Caveats
------------------------------

- All screenshots provided are static representations, the actual dashboard is fully interactive, allowing users to apply filters and slicers for a dynamic, in-depth exploration of the data and insights.

- All data used in this project is fictional but constructed to accurately reflect real-world business logic, relationships, and sales/returns scenarios.

- Monetary values are in euros (€); analysis covers a 2.5-year period (2015–2017).

- Returns are tracked by both product model and region to enable targeted loss analysis.

- Data model, table names, and field names are preserved to match the provided source files.

- Findings and recommendations are specific to the patterns present in this dataset and may not generalize to other businesses or contexts.

----------------------------------------------------------------------------------------------------------------------------------------------------

Next Steps and Stakeholder Recommendations
-------------------------------------------

1. Product Management

Prioritize a detailed review of the top five returned models, with particular attention to race bikes.

Evaluate marketing, product positioning, and quality standards for these models to address recurring return patterns.

Consider targeted improvements or adjustments for high-return models based on root causes.

2. Regional Operations

UK store managers should assess local sales and return practices, as UK locations account for the majority of return losses.

Identify and share effective return prevention strategies from regions with lower loss rates.

3. Inventory and Category Teams

Use sales-to-returns ratios to inform inventory decisions, limiting stock on models associated with high return losses.

Focus promotional efforts on bike models with consistently low return rates and strong sales performance.

-------------------------------------------------------------------------------------------------------------------------------------------------------

## Potential Follow-Up Questions
----------------------------------

Which specific customer or store characteristics are most closely linked to high return rates for race bikes or other problematic models?

Are there distinct periods, regions, or campaigns where return rates spike, suggesting opportunities for preventive action?

How do store policies or after-sales processes correlate with reduced return losses in certain regions?

Given that the youngest recorded customer is 46, what are the barriers to attracting younger buyers? What targeted marketing or product strategies could expand our reach to a younger demographic?
