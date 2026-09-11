# Beverage Retail Economic Feasibility Analysis

Economic feasibility, econometric analysis and demand forecasting for a beverage retail business using Brazilian economic and market data.

## Overview

This project combines a reproducible data pipeline, econometric demand analysis, time-series forecasting and a financial model to assess the viability and risk of a beverage retail business in Brazil.

## Objectives

- Analyze the Brazilian beverage retail market and its economic drivers.
- Build a clean, documented analytical dataset.
- Estimate econometric models and forecast sales demand.
- Evaluate the investment through NPV, IRR and payback.
- Assess uncertainty with scenarios and Monte Carlo simulation.

## Project structure

```text
data/             Original, external and processed datasets
notebooks/        Exploration and narrative analysis
src/              Reusable collection, modeling and finance code
reports/          Financial model and published figures
tests/            Automated tests for reusable code
```

Raw files are immutable: never edit a file in `data/raw/` manually. Transformations must be implemented in `src/` and produce files in `data/processed/`.

## Data sources

- IBGE (retail activity and IPCA)
- Banco Central do Brasil (macroeconomic indicators)
- Novo CAGED (employment)
- INMET (weather data)

## Workflow

1. Collect and document source data;
2. Clean and integrate a master dataset;
3. Perform exploratory and seasonal analysis;
4. Estimate econometric and forecasting models;
5. Feed the demand forecast into the financial model;
6. Evaluate scenarios, risk and investment feasibility.

## Getting started

```bash
git clone https://github.com/matheuzz19/beverage-retail-feasibility-analysis.git
cd beverage-retail-feasibility-analysis
python -m venv .venv
```

Activate the environment on Windows:

```powershell
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
jupyter lab
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for the branch, commit and pull-request workflow.

## Collaboration notes

- Do not commit credentials, local environments or temporary spreadsheet files.
- One owner at a time must edit `reports/financial_model/financial_model.xlsx`; `.xlsx` files cannot be merged safely.
- Avoid simultaneous edits to the same notebook. Move reusable notebook logic into `src/`.

## Authors

- Matheus Andrade de Oliveira
- Rafael de Souza Aquino

