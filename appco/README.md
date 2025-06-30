# AppCo Example

This example will deploy the [Istio SUSE Application Collection](https://apps.rancher.io/applications/istio). 
The app will be deployed into the `istio-system` namespace. 

```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: appcotest
  namespace: fleet-local
spec:
  repo: https://github.com/rancher/fleet-examples
  branch: master
  paths:
  - appco
```