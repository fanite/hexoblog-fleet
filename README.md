# Manifests Example

This example will deploy the [hexo blog](https://blog.ifei.me/) application.
The app will be deployed into the `website` namespace.

```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: hexo-blog
  namespace: fleet-local
  labels:
    app.kubernetes.io/name: hexo-blog-fleet
    app.kubernetes.io/component: hexo-blog
    app.kubernetes.io/created-by: fanite
spec:
  repo: git@github.com:fanite/hexoblog-fleet.git
```
