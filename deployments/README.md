gotk
=============

Bootstrap the `dev` cluster:
```
gotk bootstrap github \
  --version=v0.0.20 \
  --namespace gitops-system2 \
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

