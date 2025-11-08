# deploy-calico

Declarative Calico (Tigera Operator) deployment via ArgoCD (GitOps).

## Quick start

1. Make sure ArgoCD is running in the cluster.
2. Fork this repo and set `GITHUB_USER` env var.
3. Apply bootstrap manifests:

```bash
kubectl apply -f bootstrap/argocd-project.yaml
kubectl apply -f bootstrap/app-of-apps.yaml
Watch ArgoCD UI/CLI – Calico components will appear automatically.
