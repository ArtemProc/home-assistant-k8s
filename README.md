# home-assistant-k8s
Home-Assistant Kustomize using Fleet

```
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  name: home-assistant
  namespace: fleet-default
  labels:
    home-assistant: enabled
spec:
  branch: main
  repo: https://github.com/NicoOosterwijk/home-assistant-k8s.git
  targets:
    - clusterGroup: home-assistant
```