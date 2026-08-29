# data_pipeline/

Ingestion, validation, and feature engineering for the AML dataset.

Planned:
- `fetch_kaggle_data.py` — pulls the IBM AML dataset, produces the two client-format views (see `config/clients/`)
- `validate.py` — Great Expectations suite (schema, null, range, duplicate checks)
- `staging.py` — DuckDB staging tables
- `features.py` — risk feature engineering (velocity, structuring signals, geo risk)
- `ingestion_agent.py` — LLM agent for schema-drift / quarantine judgment calls (not per-row validation — see docs/ARCHITECTURE.md)
- `dags/ingestion_dag.py` — Airflow DAG orchestrating the above
