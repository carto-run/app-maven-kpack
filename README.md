# app-maven-kpack

## Creating the Workload

```
tanzu apps workload create app-maven-kpack \
  --namespace dev \
  --git-branch main \
  --git-repo https://github.com/carto-run/app-maven-kpack \
  --label apps.tanzu.vmware.com/has-tests=true \
  --label app.kubernetes.io/part-of=app-maven-kpack \
  --type web \
  --yes
```

## Logs

```
tanzu apps workload tail app-maven-kpack
```

## Configuration

| Item            | Config                  |
| --------------- | ----------------------- |
| Scan Policy     | Default                 |
| tap-values.yaml | na                      |
| Supply Chain    | source-test-scan-to-url |

# app-maven-kpack
