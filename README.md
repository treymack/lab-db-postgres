# lab-db-postgres

PostgreSQL experiments. Run in VSCode probably.

## Experiment Checklist

### Fundamentals

- [ ] Run Postgres in Docker (`docker run postgres`)
- [ ] Connect with `psql` and explore `\d`, `\dt`, `\di` meta-commands
- [ ] Use `EXPLAIN ANALYZE` to read query plans

### Tooling

- [ ] `pgAdmin` or `DBeaver` as a GUI
- [ ] `flyway` or `sqitch` for schema migrations
- [ ] `pgbench` for load testing
- [ ] `pg_dump` / `pg_restore` backup strategies

### Core SQL

- [ ] SELECT basics: columns, aliases, expressions, DISTINCT
- [ ] WHERE clause: comparison operators, AND/OR/NOT, BETWEEN, IN, LIKE, IS NULL
- [ ] ORDER BY and LIMIT with OFFSET
- [ ] Aggregate functions: COUNT, SUM, AVG, MIN, MAX
- [ ] GROUP BY and HAVING clauses
- [ ] Basic JOINs: INNER, LEFT, RIGHT, FULL OUTER, self-joins
- [ ] Set operations: UNION, INTERSECT, EXCEPT
- [ ] INSERT: basic, multiple rows, SELECT, RETURNING, ON CONFLICT
- [ ] UPDATE: basic, multiple columns, with expressions/subqueries, RETURNING
- [ ] DELETE: basic, with subqueries, RETURNING, TRUNCATE
- [ ] CREATE TABLE: basic table creation with PRIMARY KEY and common constraints

### Schema Management

- [ ] ALTER TABLE: add/modify/drop columns
- [ ] Rename tables and columns
- [ ] DROP TABLE, views, and indexes
- [ ] Views and materialized views
- [ ] Transactions: BEGIN, COMMIT, ROLLBACK, SAVEPOINT, isolation levels

### Data Modeling

- [ ] Table inheritance and partitioning (range, list, hash)
- [ ] JSONB columns — storage, operators, indexing with GIN
- [ ] Arrays and the `unnest()` function
- [ ] Full-text search with `tsvector` / `tsquery`

### Indexing

- [ ] B-tree vs. Hash vs. GIN vs. GiST index types
- [ ] Partial indexes (`CREATE INDEX ... WHERE ...`)
- [ ] Expression indexes (`CREATE INDEX ON t (lower(col))`)
- [ ] Index-only scans and covering indexes (`INCLUDE`)

### Advanced Queries

- [ ] Window functions (`ROW_NUMBER`, `LAG`, `LEAD`, `NTILE`)
- [ ] CTEs and recursive CTEs (`WITH RECURSIVE`)
- [ ] Lateral joins (`JOIN LATERAL`)
- [ ] `GROUPING SETS`, `ROLLUP`, `CUBE`

### Performance & Tuning

- [ ] `pg_stat_statements` for query-level metrics
- [ ] Autovacuum behavior and manual `VACUUM ANALYZE`
- [ ] Connection pooling with PgBouncer
- [ ] `work_mem`, `shared_buffers`, `effective_cache_size` tuning

### Extensions

- [ ] `pgvector` — vector similarity search
- [ ] `PostGIS` — geospatial queries
- [ ] `pg_cron` — scheduled jobs inside Postgres
- [ ] `timescaledb` — time-series workloads
- [ ] `pg_partman` — automated partition management

### Replication & HA

- [ ] Streaming replication (primary + standby)
- [ ] Logical replication and publication/subscription
- [ ] Failover with Patroni or pg_auto_failover
