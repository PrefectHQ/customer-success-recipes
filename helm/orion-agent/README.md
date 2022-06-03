# prefect-orion

![Version: 0.0.0](https://img.shields.io/badge/Version-0.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: latest](https://img.shields.io/badge/AppVersion-latest-informational?style=flat-square)

Prefect orion application bundle

**Homepage:** <https://github.com/PrefectHQ>

## Maintainers

| Name     | Email               | Url |
| -------- | ------------------- | --- |
| gabcoyne | <george@prefect.io> |     |

## Source Code

* <https://github.com/PrefectHQ/prefect-recipes>

## Requirements

| Repository                         | Name       | Version |
| ---------------------------------- | ---------- | ------- |
| https://charts.bitnami.com/bitnami | postgresql | ~9.3.2  |

## Values

| Key                                              | Type   | Default                    | Description |
| ------------------------------------------------ | ------ | -------------------------- | ----------- |
| agent.affinity                                   | object | `{}`                       |             |
| agent.autoscaling.enabled                        | bool   | `false`                    |             |
| agent.autoscaling.maxReplicas                    | int    | `10`                       |             |
| agent.autoscaling.minReplicas                    | int    | `1`                        |             |
| agent.autoscaling.targetCPUUtilizationPercentage | int    | `80`                       |             |
| agent.enabled                                    | bool   | `true`                     |             |
| agent.image.name                                 | string | `"prefecthq/prefect"`      |             |
| agent.image.pullPolicy                           | string | `"IfNotPresent"`           |             |
| agent.image.tag                                  | string | `"2.0b4-python3.8"`        |             |
| agent.nodeSelector                               | object | `{}`                       |             |
| agent.podAnnotations                             | object | `{}`                       |             |
| agent.podSecurityContext                         | object | `{}`                       |             |
| agent.replicaCount                               | int    | `1`                        |             |
| agent.resources                                  | object | `{}`                       |             |
| agent.securityContext                            | object | `{}`                       |             |
| agent.serviceAccount.annotations                 | object | `{}`                       |             |
| agent.serviceAccount.create                      | bool   | `true`                     |             |
| agent.serviceAccount.name                        | string | `""`                       |             |
| agent.tolerations                                | list   | `[]`                       |             |
| agent.workQueueName                              | string | `"kubernetes"`             |             |
| annotations                                      | object | `{}`                       |             |
| api.affinity                                     | object | `{}`                       |             |
| api.autoscaling.enabled                          | bool   | `false`                    |             |
| api.autoscaling.maxReplicas                      | int    | `100`                      |             |
| api.autoscaling.minReplicas                      | int    | `1`                        |             |
| api.autoscaling.targetCPUUtilizationPercentage   | int    | `80`                       |             |
| api.debug_enabled                                | bool   | `false`                    |             |
| api.enabled                                      | bool   | `true`                     |             |
| api.image.name                                   | string | `"prefecthq/prefect"`      |             |
| api.image.pullPolicy                             | string | `"IfNotPresent"`           |             |
| api.image.tag                                    | string | `"2.0b4-python3.8"`        |             |
| api.ingress.annotations                          | object | `{}`                       |             |
| api.ingress.className                            | string | `""`                       |             |
| api.ingress.enabled                              | bool   | `true`                     |             |
| api.ingress.hosts[0].host                        | string | `"chart-example.local"`    |             |
| api.ingress.hosts[0].paths[0].path               | string | `"/"`                      |             |
| api.ingress.hosts[0].paths[0].pathType           | string | `"ImplementationSpecific"` |             |
| api.ingress.tls                                  | list   | `[]`                       |             |
| api.nodeSelector                                 | object | `{}`                       |             |
| api.podAnnotations                               | object | `{}`                       |             |
| api.podSecurityContext                           | object | `{}`                       |             |
| api.replicaCount                                 | int    | `1`                        |             |
| api.resources                                    | object | `{}`                       |             |
| api.securityContext                              | object | `{}`                       |             |
| api.service.port                                 | int    | `4200`                     |             |
| api.service.type                                 | string | `"ClusterIP"`              |             |
| api.tolerations                                  | list   | `[]`                       |             |
| fullnameOverride                                 | string | `""`                       |             |
| imagePullSecrets                                 | list   | `[]`                       |             |
| jobs.createWorkQueue.annotations                 | object | `{}`                       |             |
| jobs.createWorkQueue.enabled                     | bool   | `false`                    |             |
| jobs.createWorkQueue.image.PullSecrets           | list   | `[]`                       |             |
| jobs.createWorkQueue.image.name                  | string | `"prefecthq/prefect"`      |             |
| jobs.createWorkQueue.image.pullPolicy            | string | `"IfNotPresent"`           |             |
| jobs.createWorkQueue.image.tag                   | string | `"2.0b4-python3.8"`        |             |
| nameOverride                                     | string | `""`                       |             |
| postgresql.existingSecret                        | string | `nil`                      |             |
| postgresql.externalHostname                      | string | `""`                       |             |
| postgresql.initdbUser                            | string | `"postgres"`               |             |
| postgresql.persistence.enabled                   | bool   | `false`                    |             |
| postgresql.persistence.size                      | string | `"8Gi"`                    |             |
| postgresql.postgresqlDatabase                    | string | `"prefect"`                |             |
| postgresql.postgresqlPassword                    | string | `""`                       |             |
| postgresql.postgresqlUsername                    | string | `"prefect"`                |             |
| postgresql.servicePort                           | int    | `5432`                     |             |
| postgresql.useSubChart                           | bool   | `true`                     |             |
| prefectVersionTag                                | string | `"2.0b4-python3.8"`        |             |
| serviceAccount.enabled                           | bool   | `true`                     |             |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.10.0](https://github.com/norwoodj/helm-docs/releases/v1.10.0)
