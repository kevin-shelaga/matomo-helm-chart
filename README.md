# Matomo Chart

Matomo is an open source alternative to Google Analytics.

## Parameters

Most relevant parameters, if you need an advanced configuration, take a look into the `values.yaml`.

| Parameter | Description | Default |
|:----------|:------------|:--------|
| `replicaCount` | How many instances of Matomo should run in parallel | `1` |
| `image.tag` | Override the version tag for the Matomo docker image | `""` (Using chart appVersion)             |
| `ingress.enabled` | Enable Ingress support | `false`  |
| `ingress.type` | Type of the ingress `default` and `traefik` are possible  | `default` |
| `ingress.annotations` | Use it for `nginx` or `traefik v1` ingress classes | `{}` |
| `ingress.hosts[].host` | host name for the ingress | `chart-example.local` |
| `ingress.hosts[].paths` | Paths for the ingress| `[ / ]` |
| `ingress.tls.default[].secretName` | If defined, TLS is enabled for the default ingress | `chart-example-tls` |
| `ingress.tls.default[].hosts` | Specify the host for the TLS certificate | `[ chart-example.local ]` |
| `ingress.tls.traefik` | If defined, traefik will use this as certificate resolver | `chart-example-tls` |
| `matomo.host` | Host of the Matomo installation | `chart-example.local` |
| `matomo.username` | Superusers name | `admin` |
| `matomo.password` | Superusers password | `My$uper$ecretPassword123#` |
| `matomo.email` | Superusers email address | `admin@chart-example.local` | 
| `matomo.website_host` | Host of the tracked website | `https://tracked-website.local` |
| `matomo.website_name` | Name of the tracked website | `Tracked Website` |
| `matomo.env` | Additional Environment variables, e.g. to configure SMTP | `{}` |



