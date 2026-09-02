# Contributing

## Branches

`main` is the stable, reviewable version. Do not commit directly to it. Create a short-lived branch from an up-to-date `main` for each Issue:

```text
feature/ibge-data
feature/sarimax-forecast
fix/npv-calculation
docs/data-sources
```

Start a task with:

```bash
git switch main
git pull origin main
git switch -c feature/short-description
```

## Commits

Use Conventional Commits, in English, written in the imperative:

```text
feat: add IBGE retail sales collector
fix: correct NPV discount rate
docs: document data sources
test: add financial model test cases
refactor: simplify preprocessing pipeline
```

Allowed types: `feat`, `fix`, `docs`, `test`, `refactor`, `chore` and `data`.

## Pull requests

Push the branch and open a pull request into `main`:

```bash
git add <files>
git commit -m "feat: add IBGE retail sales collector"
git push -u origin feature/ibge-data
```

Link the Issue in the PR description with `Closes #<number>`. The other collaborator reviews it before merging. Resolve conflicts locally, update the branch, then request review again.

## Ownership

- Data, econometrics and forecasting: `data/`, `src/data/`, `src/models/`, notebooks 01–05.
- Finance, valuation and risk: `src/finance/`, `reports/financial_model/`, notebook 06.
- Both collaborators: `README.md`, `reports/figures/` and final integration.

Do not edit the same `.ipynb` or `financial_model.xlsx` concurrently.

