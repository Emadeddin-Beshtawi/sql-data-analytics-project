# SQL Data Analytics — SQL Server

Analytics-focused SQL project built **on top of** a Medallion data warehouse (Bronze/Silver/Gold).  
This repo contains seven **T-SQL** scripts for change-over-time, cumulative trends, performance deltas, segmentation, part-to-whole, and two business reports (Customers & Products).  
The underlying DW is vendored at **`deps/data-warehouse`** (tag **v1.0.0**) so the project is self-contained.

## How to Run

1. Open scripts with the **VS Code → SQL Server** extension.
2. Make sure your active database is **`DataWarehouse`** (from `deps/data-warehouse`).
3. Run the analytics scripts in `scripts/` (order is flexible, but a common flow is 01 → 07).
4. The report scripts **06** and **07** create views:
   - `gold.report_customers`
   - `gold.report_products`
5. After running them, you can query:
   ```sql
   SELECT * FROM gold.report_customers;
   SELECT * FROM gold.report_products;

## Scripts

- `01_change_over_time_analysis.sql`
- `02_cumulative_analysis.sql`
- `03_performance_analysis.sql`
- `04_data_segmentation.sql`
- `05_part_to_whole_analysis.sql`
- `06_report_customers.sql` → creates view `gold.report_customers`
- `07_report_products.sql`  → creates view `gold.report_products`

**Query the report views:**
```sql
SELECT * FROM gold.report_customers;
SELECT * FROM gold.report_products;
