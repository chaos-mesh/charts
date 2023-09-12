![Chaos Mesh Social Preview](https://raw.githubusercontent.com/chaos-mesh/.github/main/chaos-mesh-social-preview.png)

<h1 align="center">Chaos Mesh Helm Charts</h1>

<p align="center">Helm charts for Chaos Mesh.</p>

<p align="center">
  <a href="https://chaos-mesh.org">Website</a> •
  <a href="https://chaos-mesh.org/docs/">Documentation</a> •
  <a href="https://chaos-mesh.org/docs/basic-features/">Features</a> •
  <a href="https://github.com/chaos-mesh/rfcs">RFCs</a> •
  <a href="https://slack.cncf.io/">Join our Slack channel (#project-chaos-mesh)</a>
</p>

## Overview

Chaos Mesh is an open source cloud-native Chaos Engineering platform. It offers various types of fault simulation and has an enormous capability to orchestrate fault scenarios.

Using Chaos Mesh, you can conveniently simulate various abnormalities that might occur in reality during the development, testing, and production environments and find potential problems in the system. To lower the threshold for a Chaos Engineering project, Chaos Mesh provides you with a visualization operation. You can easily design your Chaos scenarios on the Web UI and monitor the status of Chaos experiments.

## Quick Start

```sh
helm repo add chaos-mesh https://charts.chaos-mesh.org
helm install chaos-mesh chaos-mesh/chaos-mesh --namespace=chaos-mesh --create-namespace
```

## Documentation

### Prerequisites

> Since Helm 3 has been released for a while, we will only support Helm 3 in the future. If you are still using Helm 2, please upgrade to Helm 3.

- See <https://chaos-mesh.org/supported-releases/> for supported Kubernetes versions.
- Helm 3

### Using Helm

1. Add Chaos Mesh repository:

   ```bash
   helm repo add chaos-mesh https://charts.chaos-mesh.org
   ```

2. Search available version:

   ```bash
   helm search repo chaos-mesh
   ```

### Install Chaos Mesh

```bash
helm install chaos-mesh chaos-mesh/chaos-mesh --namespace=chaos-mesh --create-namespace
```

For more details about the installation and configuration, please refer to [README of chart source directory](https://github.com/chaos-mesh/chaos-mesh/tree/master/helm/chaos-mesh).

## License

Chaos Mesh is licensed under the Apache License, Version 2.0. See [LICENSE](./LICENSE) for the full license text.
