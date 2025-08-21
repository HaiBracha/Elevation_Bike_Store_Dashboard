Elevation_Bike_Store_Dashboard

Interactive Power BI dashboard analyzing sales, returns, and trends for the Elevation Bike Store project.  
Includes insights for different managerial roles, detailed return loss breakdowns, and product-level performance analysis.  
All datasets are real, not fictional.

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

---
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

## 📌 Key Insights
- **€765K in returns over 2.5 years**, with **€571K (75%)** coming from just 5 bike models.  
- **Bikes account for 96% of total return losses**, with UK stores responsible for ~€459K (60% of all losses).  
- **4 of the 5 most returned bike models are race bikes**, suggesting possible misalignment with customer expectations.  
- **A very small number of models are responsible for the majority of losses**, highlighting the need for targeted product interventions.




<img width="1290" height="731" alt="image" src="https://github.com/user-attachments/assets/f2dd9c12-20c7-4508-865a-42c67981bfc2" />

<img width="1293" height="732" alt="image" src="https://github.com/user-attachments/assets/21cc38d6-46e8-414e-87e2-156867653baa" />

<img width="1297" height="732" alt="image" src="https://github.com/user-attachments/assets/53e2a8c6-639e-4062-9902-94f8734a6cff" />

<img width="1297" height="732" alt="image" src="https://github.com/user-attachments/assets/17772d25-8ac8-40b9-a2ed-40c9ccd769b7" />

<img width="1297" height="732" alt="image" src="https://github.com/user-attachments/assets/dc242f2f-23ca-40ee-944f-e5c01403150f" />

<img width="1295" height="735" alt="image" src="https://github.com/user-attachments/assets/ca716fe5-df3e-439c-9231-c72d8e2473ca" />





