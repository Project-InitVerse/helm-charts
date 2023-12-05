# Ingress Chart

define config, create file `values.yml`
```yaml
domain: example.local #your domain
```

## Installing the Chart

To install the chart with the release name `ingress`:

```console
$ helm repo add ini https://charts.inichain.com/
"ini" has been added to your repositories

$ helm install ingress ini/ingress -f values.yml
NAME: ingress
...
```