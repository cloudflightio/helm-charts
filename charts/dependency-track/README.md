# dependency-track

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 4.10.0](https://img.shields.io/badge/AppVersion-4.10.0-informational?style=flat-square)

Install OWASP Dependency-Track on Kubernetes (or RedHat Openshift)

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| oci://registry-1.docker.io/bitnamicharts | common | 2.x.x |
| oci://registry-1.docker.io/bitnamicharts | postgresql | 13.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| apiserver.emptyDir.sizeLimit | string | `"8Gi"` |  |
| apiserver.image.pullPolicy | string | `"IfNotPresent"` |  |
| apiserver.image.repository | string | `"dependencytrack/apiserver"` |  |
| apiserver.image.tag | string | `"4.10.1"` |  |
| apiserver.persistentVolume.accessModes[0] | string | `"ReadWriteOnce"` |  |
| apiserver.persistentVolume.annotations | object | `{}` |  |
| apiserver.persistentVolume.enabled | bool | `true` |  |
| apiserver.persistentVolume.size | string | `"8Gi"` |  |
| apiserver.persistentVolume.storageClass | string | `""` |  |
| apiserver.replicaCount | int | `1` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| frontend.image.pullPolicy | string | `"IfNotPresent"` |  |
| frontend.image.repository | string | `"dependencytrack/frontend"` |  |
| frontend.image.tag | string | `"4.10.0"` |  |
| frontend.replicaCount | int | `1` |  |
| fullnameOverride | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.host | string | `"example.com"` |  |
| ingress.openshift | bool | `false` |  |
| ingress.tls.enabled | bool | `false` |  |
| ingress.tls.secretName | string | `""` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| oidc.enabled | bool | `false` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| postgresql.auth.database | string | `"dependencytrack"` |  |
| postgresql.auth.password | string | `"dependencytrack"` |  |
| postgresql.auth.username | string | `"dependencytrack"` |  |
| postgresql.enabled | bool | `true` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.port | int | `8080` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |

