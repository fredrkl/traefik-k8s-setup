# Traefik v2 on AKS sample

Demo on setting up Traefik in K8s. This demo also spins up a new AKS cluster.

## Setup

1. Clone/Fork this repo
2. Create an RG in Azure and note down the name
3. Create a GitHub secret holding an Azure Service Principal following this guide: <https://github.com/Azure/actions-workflow-samples/blob/master/assets/create-secrets-for-GitHub-workflows.md> giving it access to the RG in step 2.
4. Kick off the GitHub action

[![Create Traefik demo AKS cluster](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/createaks.yml/badge.svg)](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/createaks.yml)

[![Deploy to AKS](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/deploy-to-aks.yml/badge.svg)](https://github.com/fredrkl/traefik-k8s-setup/actions/workflows/deploy-to-aks.yml)
