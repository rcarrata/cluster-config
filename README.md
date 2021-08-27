# Cluster Config

Cluster Config of Openshift4 Clusters using GitOps

## Clone the repo

```
git clone https://github.com/rcarrata/cluster-config.git
cd cluster-config
```

## Install Openshift GitOps with Dex OAuth

```
until oc apply -k bootstrap/; do sleep 2; done
```

## Deploy the Cluster Config in ArgoCD

```
oc apply -k cluster-config/config/overlays/default/
```

<img align="center" width="750" src="assets/pic1.png">

