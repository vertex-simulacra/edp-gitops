# GitOps

This repository contains the GitOps configuration for the `Applications` that are deployed in the cluster. One can override the default values of the applications helm-chart by creating a file with the name `<application-name>-values.yaml` in the respective folder. Check for more details in the [platform documentation](https://epam.github.io/edp-install/user-guide/gitops/#gitops-usage)

Structure of the repository is as follows:

```bash
<pipeline-name>/<stage-name>/<application-name>-values.yaml
```

For example:

```bash
├── delivery
│   ├── qa
│   │   ├── cart-service-values.yaml
│   │   ├── frontend-values.yaml
│   │   ├── payment-gateway-service-values.yaml
│   │   └── user-service-values.yaml
│   ├── sit
│   │   ├── cart-service-values.yaml
│   │   ├── frontend-values.yaml
│   │   ├── payment-gateway-service-values.yaml
│   │   └── user-service-values.yaml
│   └── uat
│       ├── cart-service-values.yaml
│       ├── frontend-values.yaml
│       ├── payment-gateway-service-values.yaml
│       └── user-service-values.yaml
├── feature1
│   ├── dev
│   │   ├── payment-gateway-service-values.yaml
│   │   └── user-service-values.yaml
│   ├── qa
│   │   ├── payment-gateway-service-values.yaml
│   │   └── user-service-values.yaml
│   └── uat
│       ├── payment-gateway-service-values.yaml
│       └── user-service-values.yaml
└── mypipeline
    ├── dev
    │   ├── cart-service-values.yaml
    │   ├── frontend-values.yaml
    ├── qa
    │   ├── cart-service-values.yaml
    │   ├── frontend-values.yaml
    ├── sit
    │   ├── cart-service-values.yaml
    │   ├── frontend-values.yaml
    └── uat
        ├── cart-service-values.yaml
        └── frontend-values.yaml
```
