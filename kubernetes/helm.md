# Helm

## Commands:

I. Repository

```
helm repo list
```

II. Create chart

```
helm create lab-mock-server
```

III. Check chart

```
helm lint lab-mock-server
```

IV. Install chart with namespace

For default the pod name is concatenated with namespace.
For custom name use:

- `nameOverride`: "lab-mock-server"
- `fullnameOverride`: "lab-mock-server"

```
helm install lab-mock-server  ./lab-mock-server --namespace laboratory
```

V. List chart

```
helm list -n laboratory
```

VI. Uninstall chart with namespace

```
helm uninstall mysite --namespace laboratory
```