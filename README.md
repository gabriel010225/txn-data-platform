# txn-data-platform
Simulated card-transaction platform: streaming ingestion, real-time features and fraud scoring, plus batch modelling with dbt and Airflow.

## Goal
Build an end-to-end data platform the way a bank would: idempotent ingestion, tested data models, real-time scoring and alerting, scheduled batch jobs.

## Data
Synthetic transactions generated with Faker. No real customer data.

## Planned architecture
Python producer -> Redpanda (Kafka API) -> consumer -> Postgres -> dbt models.
Real-time window features -> fraud scoring (fraud-detection API) -> alerts table -> LLM daily risk report.
Airflow schedules the batch jobs and data quality checks.

## Status
- [ ] Docker and Redpanda running locally
- [ ] Transaction producer
- [ ] Consumer writing to Postgres

## How to run
To be added.
