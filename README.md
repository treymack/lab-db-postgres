# lab-db-postgres

PostgreSQL experiments. Run in VSCode probably.

## Experiment Checklist

### Fundamentals

- [ ] Run Postgres in Docker (`docker run postgres`)
- [ ] Connect with `psql` and explore `\d`, `\dt`, `\di` meta-commands
- [ ] Use `EXPLAIN ANALYZE` to read query plans

### Indexing

- [ ] B-tree vs. Hash vs. GIN vs. GiST index types
- [ ] Partial indexes (`CREATE INDEX ... WHERE ...`)
- [ ] Expression indexes (`CREATE INDEX ON t (lower(col))`)
- [ ] Index-only scans and covering indexes (`INCLUDE`)

### Data Modeling

- [ ] Table inheritance and partitioning (range, list, hash)
- [ ] JSONB columns — storage, operators, indexing with GIN
- [ ] Arrays and the `unnest()` function
- [ ] Full-text search with `tsvector` / `tsquery`

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

### Replication & HA

- [ ] Streaming replication (primary + standby)
- [ ] Logical replication and publication/subscription
- [ ] Failover with Patroni or pg_auto_failover

### Extensions

- [ ] `pgvector` — vector similarity search
- [ ] `PostGIS` — geospatial queries
- [ ] `pg_cron` — scheduled jobs inside Postgres
- [ ] `timescaledb` — time-series workloads
- [ ] `pg_partman` — automated partition management

### Tooling

- [ ] `pgAdmin` or `DBeaver` as a GUI
- [ ] `pgbench` for load testing
- [ ] `pg_dump` / `pg_restore` backup strategies
- [ ] `flyway` or `sqitch` for schema migrations
