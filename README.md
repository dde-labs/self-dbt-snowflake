# Self: DBT with Snowflake

Self Sandbox for develop **DBT & Snowflake** connector

## Prerequisite

This project use Python version 3.9 and then you should install all deps;

```shell
pip install -r requirements.txt
```

> [!NOTE]
> For decrease installation time, it should use `uv`.

# Components of DBT

- **Models**: This is where you write your SQL models.
- **Tests**: This is where you can store your data.
- **Macros**: This is where you can define macros to simplify your SQL code.
- **Analysis**: This is where you can write SQL code to analyze your data.
- **Logs**: These are run logs. They are generated when a ‘dbt run’ command is executed.
- **Target Directories** (e.g. dev): Either when compiling, running or building
  documentation, these are created. They contain all of the meta content and
  compiled SQL code.

## Tips

I learn tips from [DBT(data build tool) EP: 01](https://aumt3.medium.com/dbt-data-build-tool-ep-01-adb58297e788)
