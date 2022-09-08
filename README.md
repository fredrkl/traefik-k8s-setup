# Traefik v2.8.4 on Kubernetes (K8s) sample

Demo on setting up Traefik in K8s. This demo also spins up a new MS AKS cluster.

## Setup

1. Clone/Fork this repo
2. Create an RG in Azure and note down the name
3. Create a GitHub secret holding an Azure Service Principal following this guide: <https://github.com/Azure/actions-workflow-samples/blob/master/assets/create-secrets-for-GitHub-workflows.md> giving it access to the RG in step 2.
4. Kick off the _Deploy to AKS_ GitHub action to create AKS

![Traefik](/images/traefik-logo.png)

## Tips

- If you want to use [middlewares](https://doc.traefik.io/traefik/middlewares/overview/) in K8s, you need to enable the KubernetesCRD provider regardless, even if you use the KubernetesIngress provider for Traefik configuration, e.g,. <https://github.com/fredrkl/traefik-k8s-setup/commit/fcdba1a878c815249e07ba711a0e9429572882ff>

## Workflows

[![Create Traefik demo AKS cluster](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/createaks.yml/badge.svg)](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/createaks.yml)

[![Deploy to AKS](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/deploy-to-aks.yml/badge.svg)](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/deploy-to-aks.yml)
