# ng-manager

![Version: 0.2.13](https://img.shields.io/badge/Version-0.2.13-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.1](https://img.shields.io/badge/AppVersion-0.0.1-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.bitnami.com/bitnami | common | 2.x.x |
| https://harness.github.io/helm-common | harness-common | 1.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| appLogLevel | string | `"INFO"` |  |
| autoscaling.enabled | bool | `true` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| fullnameOverride | string | `""` |  |
| global.loadbalancerURL | string | `""` |  |
| image.digest | string | `""` |  |
| image.imagePullSecrets | list | `[]` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"harness/ng-manager-signed"` |  |
| image.tag | string | `"76019"` |  |
| imagePullSecrets | object | `{}` |  |
| initContainer.image.digest | string | `""` |  |
| initContainer.image.imagePullSecrets | list | `[]` |  |
| initContainer.image.registry | string | `"docker.io"` |  |
| initContainer.image.repository | string | `"busybox"` |  |
| initContainer.image.tag | string | `"1.35.0"` |  |
| java.memory | string | `"4096m"` |  |
| maxSurge | int | `1` |  |
| maxUnavailable | int | `0` |  |
| mongoSecrets.password.key | string | `"mongodb-root-password"` |  |
| mongoSecrets.password.name | string | `"mongodb-replicaset-chart"` |  |
| mongoSecrets.userName.key | string | `"mongodbUsername"` |  |
| mongoSecrets.userName.name | string | `"harness-secrets"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | int | `2` |  |
| resources.limits.memory | string | `"8192Mi"` |  |
| resources.requests.cpu | int | `2` |  |
| resources.requests.memory | string | `"200Mi"` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `65534` |  |
| service.gitsyncgrpcport | int | `13002` |  |
| service.grpcport | int | `9979` |  |
| service.port | int | `7090` |  |
| service.protocol | string | `"TCP"` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| timescaleSecret.password.key | string | `"timescaledbPostgresPassword"` |  |
| timescaleSecret.password.name | string | `"harness-secrets"` |  |
| tolerations | list | `[]` |  |
| waitForInitContainer.image.digest | string | `""` |  |
| waitForInitContainer.image.imagePullSecrets | list | `[]` |  |
| waitForInitContainer.image.pullPolicy | string | `"IfNotPresent"` |  |
| waitForInitContainer.image.registry | string | `"docker.io"` |  |
| waitForInitContainer.image.repository | string | `"harness/helm-init-container"` |  |
| waitForInitContainer.image.tag | string | `"latest"` |  |

