# Data warehouse
In computing, a data warehouse, also known as an enterprise data warehouse, is a system used for reporting and data analysis, and is considered a core component of business intelligence. DWs are central repositories of integrated data from one or more disparate sources

![Data Mart](Data_Warehouse.jpg)


---

## Slowly Changing Dimensions (SCD) Types

- Type 0 – Fixed Dimension
No changes allowed, dimension never changes

- Type 1 – No History
Update record directly, there is no record of historical values, only current state

- Type 2 – Row Versioning
Track changes as version records with current flag & active dates and other metadata

- Type 3 – Previous Value column
Track change to a specific attribute, add a column to show the previous value, which is updated as further changes occur

- Type 4 – History Table
Show current value in dimension table but track all changes in separate table

- Type 6 – Hybrid SCD
Utilise techniques from SCD Types 1, 2 and 3 to track change
