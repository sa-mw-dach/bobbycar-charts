# Bobbycar Helm Charts

Helm Chart repository for the Bobbycar demonstrator:

## Core Charts:

- bobbycar-core-infra
- bobbycar-core-apps
- bobbycar-opt-serverless

## Optional Charts:

- bobbycar-opt-dev-base
- bobbycar-opt-dev-pipelines

### Update and index the repo

```sh
helm repo index docs/ --url https://sa-mw-dach.github.io/bobbycar-charts
```