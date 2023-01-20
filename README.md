
# Deploy to Kubernetes with Kustomize

This is a sample web application that uses Kustomize to deploy to different environments (production and staging).

## Deploy Locally

To deploy locally (with kubectl 1.14+), run the following:

`kubectl apply -k overlays/staging`

`kubectl apply -k overlays/production`

If using an older version of kubectl, use:

`kustomize build overlays/staging | kubectl apply -f`

`kustomize build overlays/production | kubectl apply -f`


