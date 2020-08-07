# Chaos Mesh Helm repository

Add Chaos Mesh repository to Helm repos:

```bash
helm repo add chaos-mesh https://charts.chaos-mesh.org
```

Search avaliable version: 

```bash
helm search repo chaos-mesh
```
## Create custom resource type

To use Chaos Mesh, you must create the related custom resource type.

```bash
curl -sSL https://raw.githubusercontent.com/chaos-mesh/chaos-mesh/master/manifests/crd.yaml | kubectl apply -f - 
```

## Install Chaos Mesh

  - For helm 2.X

```bash
helm install chaos-mesh/chaos-mesh --name=chaos-mesh --namespace=chaos-testing
```

- For helm 3.X

```bash
helm install chaos-mesh chaos-mesh/chaos-mesh --namespace=chaos-testing
```

For more details on installing Chaos Mesh please see the [chart readme](https://github.com/pingcap/chaos-mesh/tree/master/helm/chaos-mesh).

