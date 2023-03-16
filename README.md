# Local testing: Kyverno installation by ArgoCD

Following the argocd-envs repository:
- environment folder contains all argo cd applications.
- app-stacks folder contains the stacks "applications" needed by the software that you want to install on cluster
- components folder contains all the manifests to be installed.

## Installation process:

In "environment" kyverno.yaml is an ArgoCD application pointing in this repository at the following paths:

- **/app-stacks/kyverno-app.yaml** : ArgoCD Application that installs kyverno engine
- **/app-stacks/kyverno-monitor.yaml**: ArgoCD Application that installs the monitor
- **/app-stacks/kyverno-policies.yaml**: ArgoCD Application that installs the policies (inside the components folder)

## kyverno: TODO

## CloudnativePG:
### Installation
