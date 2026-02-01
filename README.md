# Discussion #34109

Reproduction for [renovate discussion #34109](https://github.com/renovatebot/renovate/discussions/34109)

## Current behavior

Missing changelog for the package `registry.k8s.io/ingress-nginx/controller`. The changelog is only shown for the `ingress-nginx` package. See https://github.com/philipfreude/ingress-nginx-renovate/pull/1.

The changelog is discarded by renovate with the following log message
```
DEBUG: Fetching changelog: https://github.com/kubernetes/ingress-nginx (4.11.3 -> 4.14.2) (repository=philipfreude/ingress-nginx-renovate, branch=renovate/ingress-nginx-group)
DEBUG: Fetching changelog: https://github.com/kubernetes/ingress-nginx (v1.11.3 -> v1.14.2) (repository=philipfreude/ingress-nginx-renovate, branch=renovate/ingress-nginx-group)
DEBUG: Removing duplicate release notes (repository=philipfreude/ingress-nginx-renovate, branch=renovate/ingress-nginx-group)
       "depName": "registry.k8s.io/ingress-nginx/controller"
```

## Expected behavior

Both the helm chart and the container within the group have a changelog in the PR description.
