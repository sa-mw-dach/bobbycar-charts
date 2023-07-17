# Red Hat Connected Vehicle Solution Pattern Helm Charts

Helm Chart repository for the Connected Vehicle Solution Pattern (aka Bobbycar):

## Core Solution Pattern Charts:

- bobbycar-core-infra
- bobbycar-core-apps
- bobbycar-opt-serverless

## Optional Solution Pattern Charts:

- bobbycar-opt-dev-base
- bobbycar-opt-dev-pipelines

### How to package the Helm Charts and update the Chart repository

First upate the Chart's `version` and the `appVersion` in the respective `Chart.yaml` file in the [Bobbycar Git Repository](https://github.com/sa-mw-dach/bobbycar/tree/master/helm). The `appVersion` is meant to reflect the OCP version the package was tested on.
Then package the Helm Chart as `.tgz` file and copy the file to this Git repo into the `/docs` folder, i.e.:

```sh
helm package helm/bobbycar-core-apps/
```

Update the index file of this repository and commit the new Charts and index file:

```sh
helm repo index docs/ --url https://sa-mw-dach.github.io/bobbycar-charts
```