# manifests
If you don't know what you're doing and/or not authorized by Warren Snipes to change something please **DO NOT**.

## Stack

- [PostgreSQL](https://www.postgresql.org/) - [_repo_](https://github.com/bitnami/charts/tree/master/bitnami/postgresql)
- [KnightHacks Microservices](https://github.com/KnightHacks/knighthacks_backend)
- [FluxCD](https://fluxcd.io/)

## Debugging

### Kustomize
To test if your kustomize changes will work out use the following command in the directory you want to test:
```bash
kubectl kustomize
```

### Flux
To follow logs as they come use the following command:
```bash
flux logs --follow
```

To get the status of your kustomizations use the following command:
```bash
flux get kustomizations -A
```

To force a reconciliation of a specific kustomization live use the following command:
```bash
flux reconcile kustomization apps
```
