gotk
=============

Bootstrap the `dev` cluster:
```
gotk bootstrap github \
  --version=v0.0.22 \
  --namespace gitops-system3 \
  --components=source-controller,kustomize-controller,helm-controller,notification-controller \
  --owner=$GITHUB_USER \
  --hostname=github.com \
  --owner=sekka1 \
  --repository=kubernetes-common-services \
  --path=deployments/aws/dev \
  --private=true \
  --interval=1m \
  --personal
```

