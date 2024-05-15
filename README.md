# Cloudflight Helm-Charts

This repository contains some of our internally and externally used helm-charts. Our favorized way to deploy services on kubernetes is Grafana Tanka and Jsonnet, but for some deployments Helm has some benefits.

## Usage

Add repository:

```shell
helm repo add cloudflight https://cloudflightio.github.io/helm-charts
```

View available charts:

```shell
helm search repo cloudflight
```

## Charts

### Dependency Track

This is mainly to provide and develop a openshift compatible chart for dependency-track.

**Why Helm and not Tanka?**

There is an official Helm-Chart of Dependency-Track (https://github.com/DependencyTrack/helm-charts/tree/main) but it is in an early stage and might not work on our openshift setup. We try to upstream our changes in the long-run but for now we will wait for the official helm-chart to stabilize.

---

#### Disclaimer

This Helm chart is provided under the Apache License 2.0. It is made available by Cloudflight "as is" and without any warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose.

Cloudflight provides this chart as a courtesy to the user community and is not obligated to provide any support, updates, or enhancements. Cloudflight is not responsible for any damages or issues that may arise from the use of this chart.

Please note that by using this chart, you agree that you do so at your own risk and you are solely responsible for any consequences that arise from its use.

#### License

This project is licensed under the Apache License 2.0. For more details, see the LICENSE file included with this chart.
