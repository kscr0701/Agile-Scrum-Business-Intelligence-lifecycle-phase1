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
 
## sprint 3 Review: Feature Delivery

The working prototype delivered at the end of sprint 3 contains 6 distinct operational sheeets. Each layout maps directly back to a PBI and business requirement:

### Sheet 1: AOV & Profit Margin
* **Agile Mapping:** Delivers
  **PBI-03** (Financial Engine metrics tracking)
* **Technical execution:** Built using explicit DAX measures to track absolute variations in AOV and net profit margin.

### Sheet 2: Top & Bottom line Financial matrix
* **Agile Mapping:** Delivers
**BR-01 / CFO Financial health Mandate**
* **Technical execution:** A comprehensive matrix breakdown of gross sales, COGS and net revenue.
  This sheet provide immediate financial transparency, revealing that whiel top-line revenue scales, minor category costs are heavily compressing absolute bottom line profit.

### Sheet 3: Return rate Analytics (Operational risk)
* **Agile Mapping:** Delivers
**PBI-04** (Comparative baseline benchmarking).
* **The strategic discovery:** This layout utilizes custom parent metrics (`return rate compared to electronics`). It explicitly exposes the **grocery category trap**, proving it holds a high return rate 61.58% of baseline) while contributing practically nothing (0.36%) to corporate profit.

### Sheet 4: Age group analysis (Customer segmentation)
* **Agile Mapping:** Delivers
**PBI-05** (Marketing demographic targeting tiers)
* **Technical execution:** This view segments purchasing volume by clean 10 year age buckets, completely resloving the mixed-string calculation bugs identified during development sprints.

### Sheet 5: Avg order drequency by state (Geographic Tracking)
* **Agile Mapping:** Delivers
**PBI-06** (universal interactve filtering)
  * **Techincal Execution:** Integrates regional and geographic dimension. Stakeholders can evaluate regional supply chain and logistics performance.
 
### Sheet 6: Electronics sales deep dive
* **Agile Mapping:** Product backlog sub task (Primary revenue Driver optimization).
* **Technical Execution**
Dedicated analytical page isolating sub-categories. This sheet ensures marketing and supply chain executives can micromanage the company's primary engine of growth. 
