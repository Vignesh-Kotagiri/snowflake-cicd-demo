# Snowflake CI/CD Demo

This is a simple proof of concept for automating Snowflake deployments using GitHub Actions.

## 🚀 Workflow
1. Push SQL scripts to the `main` branch.
2. GitHub Actions automatically runs the workflow.
3. The workflow connects to Snowflake using credentials stored in GitHub Secrets.
4. Executes SQL scripts to create and populate tables.

## 🔑 Required GitHub Secrets
Go to your repository → Settings → Secrets → Actions → New repository secret:
- `SNOWFLAKE_ACCOUNT` – Your Snowflake account identifier (e.g., abcd-xy12345)
- `SNOWFLAKE_USER` – Username
- `SNOWFLAKE_PASSWORD` – Password
- `SNOWFLAKE_WAREHOUSE` – Warehouse name
- `SNOWFLAKE_DATABASE` – Database name
- `SNOWFLAKE_SCHEMA` – Schema name
