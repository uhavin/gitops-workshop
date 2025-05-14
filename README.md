# GitOps / Flux

?

## Sample deploy

> export KEY_FP=XXXXX  
> export GITHUB_TOKEN=XXXXXX  
> export GITHUB_USER=jelmerde  
> flux bootstrap github --owner=$GITHUB_USER --repository=flux-k8s --branch=main --path=./clusters/mgmt --components-extra=image-reflector-controller,image-automation-controller --personal  
> gpg --export-secret-keys --armor "${KEY_FP}" | kubectl create secret generic sops-gpg --namespace=flux-system --from-file=sops.asc=/dev/stdin  

