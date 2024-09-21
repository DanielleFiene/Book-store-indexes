# Book-store-indexes

# SQL Skills Overview

## Key Skills

- **SQL Querying**: Proficient in retrieving data using `SELECT` statements.
- **Index Management**: Experienced in creating and managing indexes to optimize performance.
- **Performance Analysis**: Utilizes `EXPLAIN ANALYZE` for query optimization.
- **Data Size Management**: Monitors table sizes with functions like `pg_size_pretty`.
- **Data Import/Export**: Skilled in using the `\COPY` command for data management.
- **Index Cleanup**: Maintains database efficiency by removing unnecessary indexes.
- **Timestamp Functions**: Utilizes functions like `NOW()` for date and time handling.

## Example Queries

1. **Data Retrieval**:
   ```sql
   SELECT * FROM customers LIMIT 10;
   ```

2. **Index Creation**:
   ```sql
   CREATE INDEX idx_orders_customer_id ON orders (customer_id);
   ```

3. **Performance Analysis**:
   ```sql
   EXPLAIN ANALYZE SELECT original_language, title FROM books WHERE original_language = 'French';
   ```

4. **Data Import**:
   ```sql
   \COPY orders FROM 'orders_add.txt' DELIMITER ',' CSV HEADER;
   ```
