# Chaos Mesh Helm repository

Add Chaos Mesh repository to Helm repos:

```bash
helm repo add chaos-mesh https://charts.chaos-mesh.org
```

Search available version: 

```bash
helm search repo chaos-mesh
```

## Install Chaos Mesh

  - For helm 2.X

```bash
helm install chaos-mesh/chaos-mesh --name=chaos-mesh --namespace=chaos-testing
```

- For helm 3.X

```bash
kubectl create ns chaos-testing
helm install chaos-mesh chaos-mesh/chaos-mesh --namespace=chaos-testing
```

For more details on installing Chaos Mesh please see the [chart readme](https://github.com/pingcap/chaos-mesh/tree/master/helm/chaos-mesh).

