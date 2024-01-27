# home-assistant-k8s
Home-Assistant Kustomize using Fleet

```
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: kustomize
  namespace: fleet-local
spec:
  repo: https://github.com/NicoOosterwijk/home-assistant-k8s.git
  paths:
  - ./kustomize
```