# Bobbycar Helm Charts

Helm Chart repository for the Bobbycar demonstrator:

## Core Charts:

- bobbycar-core-operators
- bobbycar-core-infra
- bobbycar-core-apps

## Optional Charts:

- bobbycar-opt-serverless
- bobbycar-opt-dev-base

### Update and index the repo

```sh
helm repo index docs/ --url https://sa-mw-dach.github.io/bobbycar-charts
```