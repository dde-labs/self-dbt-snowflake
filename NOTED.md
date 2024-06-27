# NOTED

## Initialize DBT

Start create the DBT project at the first time

```shell
dbt init lakehouse
cd ./lakehouse
```

## Initialize Snowflake

Create Schema on the target Database

```sql
USE DATABASE POC;
CREATE SCHEMA dbt;
```

Allow MFA on your user if you set MFA authentication

```sql
ALTER ACCOUNT SET ALLOW_ID_TOKEN = true;
ALTER ACCOUNT SET allow_client_mfa_caching = true;
```

## Getting Started

### Setting Environment Vars

You should consider at least using an environment variable name prefixed by `DBT_ENV_SECRET_`
so that dbt keeps them out of logs. See [the docs](https://docs.getdbt.com/reference/dbt-jinja-functions/env_var#secrets) for more info

**Ubuntu**:

```text
export DBT_ENV_SECRET_*='???'
```

**Windows**:

```text
$env:DBT_ENV_SECRET_*='???'
```

### DBT

```shell
dbt run
```

## Docs

```shell
dbt docs generate
dbt docs serve
```
