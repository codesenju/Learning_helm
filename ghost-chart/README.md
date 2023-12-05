# ghost

A Helm chart for ghost/nginx/httpd

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 4.24.1](https://img.shields.io/badge/AppVersion-4.24.1-informational?style=flat-square)

## Installing the Chart

To install the chart with the release name `my-release`:

```console
helm upgrade -i my-release . -n ghost --create-namespace
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| ghost.containerPort | int | `80` | Container port |
| ghost.image | string | `"nginx:alpine"` | Container image |
| ghost.replicas | int | `1` | Number of pod replicas |
| ingress.annotations | object | `{}` | Pod annotations to add |
| ingress.hostname | string | `"ghost.demo"` | Application hostname for external access |
| ingress.ingressClassName | string | `"traefik"` | ingressClassName |

----------------------------------------------