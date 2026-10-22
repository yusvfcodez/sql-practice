# sql-practice

Learning SQL by asking questions of a realistic database.

Every query here starts as a plain-English question about a DVD-rental business, then gets answered in PostgreSQL, from simple filters up to joins, CTEs, window functions and query plans.

## Get it running
1. Install PostgreSQL and create the database:
   ```bash
   createdb dvdrental
   ```
2. Download the DVD rental sample database (`dvdrental.tar`) from the PostgreSQL Tutorial site and restore it:
   ```bash
   pg_restore -U postgres -d dvdrental /path/to/dvdrental.tar
   ```
3. Run any query file:
   ```bash
   psql -U postgres -d dvdrental -f queries/01_select_basics.sql
   ```

The dump itself is not committed to this repository.

## How it's organised
```
queries/   one .sql file per topic; each query is preceded by the question it answers
```

## The path
| File | Topic | Status |
|---|---|---|
| `01_select_basics.sql` | SELECT, WHERE, ORDER BY, LIMIT | Planned |
| `02_aggregates.sql` | COUNT, SUM, GROUP BY, HAVING | Planned |
| `03_joins.sql` | INNER, LEFT, self joins | Planned |
| `04_subqueries_ctes.sql` | Subqueries, CTEs | Planned |
| `05_window_functions.sql` | ROW_NUMBER, RANK, running totals | Planned |
| `06_indexing.sql` | EXPLAIN ANALYZE, indexes | Planned |

## License
MIT

