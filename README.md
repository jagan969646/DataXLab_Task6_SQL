# Task 6 - Sales Trend Analysis

## Summary
Aggregate monthly revenue and order volume from `orders` table and produce top months.

## Files
- task6_sales_trend.sql   -- SQL script (Postgres / MySQL / SQLite variants)
- results.csv             -- Exported result table
- screenshot.png          -- Screenshot of SQL run + results
- README.md               -- This file

## How to run (Postgres example)
1. psql -d mydb -f task6_sales_trend.sql
2. \copy (SELECT ...) TO 'results.csv' CSV HEADER

## Notes
- NULL `amount` handled with COALESCE(amount,0)
- Unique orders counted with COUNT(DISTINCT order_id)
## Author
Jagadeesh.N
jagadeesh.n10d@gmail.com
