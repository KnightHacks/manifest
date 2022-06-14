# manifests

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
