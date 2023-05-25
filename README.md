## Example Voting App Kubernetes

It can work on the Kubernetes cluster.
## Run the app in Kubernetes

The folder K8-specs contains the YAML specifications of the Voting App's services.

Run the following command to create the deployments and services. Note it will create these resources in your current namespace (`default` if you haven't changed it.)

```shell
kubectl create -f K8-specs
```

The `vote` web app is then available on port 30004 on each host of the cluster, the `result` web app is available on port 30005.

To remove them, run:

```shell
kubectl delete -f K8-specs


