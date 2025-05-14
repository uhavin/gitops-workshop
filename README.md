# GitOps / Flux

## Sample deploy

> export GITHUB_TOKEN=XXXXXX  
> export GITHUB_USER=<USERNAME>  
> flux bootstrap github --owner=$GITHUB_USER --repository=gitops-workshop --branch=main --path=./clusters/my-cluster --components-extra=image-reflector-controller,image-automation-controller --personal  
