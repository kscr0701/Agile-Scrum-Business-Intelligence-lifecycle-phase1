# Technical Implementation, Data insights & sprint Review
**Project:** Cross-channel retail profitabilityecosystem
**lifecycle phase:** Phase 1 
**Role:** Scrum practitioner/ Agile business analyst

-- 

# 1. Data Architecture: The star schema prototype
To satisfy **PBI- 02 (Data modelling)**, the team broke down flat legacy data structures into a fully optimized relational Star schema. This design ensures that dimensions
tables cleanly filter the central transactional fact table without inflating row counts or fracturing calculation logic.

* `Customer[CustomerID]` - `Sales_fact[CustomerID]`
*  `Products[ProductID]` - `Sales_fact[ProductID]`
*  `Stores[StoreID]` - `Sales_fact[StoresID]`

 --

 # 2. Sprint Implementation & Bug log 
 As scrum practitioner/BA, I tracked quality control and documented structural roadblocks during technical delivery.
 
