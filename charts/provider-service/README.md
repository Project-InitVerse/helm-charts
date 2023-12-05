# Provider Service Chart

define config, create file `values.yml`
```yaml
config:
  config.json: |
    {
      "NodeURL": "https://rpc-devnet.iniscan.com/",
      "CPUPrice": "1000000000",
      "DeploymentIngressDomain": "ingress.test3.ubicloud.matrixlabs.org",
      "MemoryPrice": "10000000",
      "StoragePrice": "1000000",
      "SecretKey": "e3a743aeaa54b9e1567625f03da306b5452a471eb01258b537fa067f06a9f890",
      "ClusterPublicHostname": "test3.ubicloud.matrixlabs.org",
      "Cert": "I44Es9V4aKKdcSfZAweN2rWkchiLr2JDFD6gx5K7DkXYJ1rhXJLcx6zSr",
      "NodeChainID": 237,
      "GatewayListenAddress": "0.0.0.0:8442",
      "DeploymentIngressExposeLBHosts": "false",
      "DeploymentIngressStaticHosts": "true",
      "DeploymentNetworkPoliciesEnabled": "true",
      "OrderFactory": "I43Pu2y1t83ShvApZUDeCTzdL1mRAwTJgXQtH5qR4yQ1aoDZeNEkgT6ih",
      "ProviderContract": "I45t2yHs2bpDJnyUm3vg9hxd29McE7YiukVGPiNL7erK4TvPDCQrxvL56",
      "OvercommitPercentCPU": "0",
      "ProviderFactoryContract": "I43Psbq3enwAmwXGa2QejWFdd9AwV1rczE6w1GPzs6WTPmJpKbmXAsdgn",
      "OvercommitPercentMemory": "0",
      "ProviderAddress": "I44Q5ErnB59SmieDpADpBadWdLkawcakgFZs8DmfERqNQMPLaCgQsF44g",
      "OvercommitPercentStorage": "0",
      "ValidatorFactoryContract": "I43Psbq3enwAmwXGa2QejWFdd9AwV1rczE6w1GPzs6WTPmJpKbmXzKEho",
      "BidTimeOut": "600",
      "NameSpace": "ubic-service",
      "HostNameServiceListenAddr": "0.0.0.0:28442",
      "HostPruneInterval": "600",
      "HostWebRefreshInterval": "5",
      "HostRetryDelay": "3",
      "DeploymentRuntimeClass": "",
      "DockerImagePullSecretsName": ""
    }
```

## Installing the Chart

To install the chart with the release name `provider-service`:

```console
$ helm repo add ini https://charts.inichain.com/
"ini" has been added to your repositories

$ helm install provider-service ini/provider-service -f values.yml
NAME: provider-service
...
```