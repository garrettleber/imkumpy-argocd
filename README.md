# imkumpy-argocd

A repo which contains my ArgoCD application manifests and related kubernetes manifests for some of my self-hosted applications

## DEPRECATION NOTICE

I no longer use kubernetes to host any of my persistent self-hosted services, I've switched to much simpler deployments using Proxmox VMs and Ansible Playbooks to lower management overhead.

I do keep the kubernetes stack running to lab on :)

## Getting Started

To create all apps in a new cluster

```bash
kubectl apply -f apps.yaml
```

