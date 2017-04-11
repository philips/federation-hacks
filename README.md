# federation-hacks

Get the [kubefed tool](https://kubernetes.io/docs/tutorials/federation/set-up-cluster-federation-kubefed/).

Deploy the federation API server:

```

```

Start the kubectl proxy to the target cluster:

```

```

Join the fake clusters and ignore any errors:

```
kubefed join cluster1 --cluster-context=fed --kubeconfig=kubeconfig  -v=10
kubefed join cluster2 --cluster-context=fed --kubeconfig=kubeconfig  -v=10
kubefed join cluster3 --cluster-context=fed --kubeconfig=kubeconfig  -v=10
```


curl  http://127.0.0.1:8001/api/v1/proxy/namespaces/default/services/warped-dragon-federation-etcd-operator:80/apis/federation/v1beta1/clusters


