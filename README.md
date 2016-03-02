# Teamcity Kubernetes

Simple scripts to set up TeamCity on Kubernetes, adapted from [here](https://tech.small-improvements.com/2015/04/09/running-teamcity-on-kubernetes/).

# Installation

```
gcloud container clusters create -m n1-standard-1 teamcity
kubectl create -f teamcity-rc.json
kubectl create -f teamcity-service.json
kubectl create -f teamcity-agent-rc.json
kubectl create -f teamcity-loadbalancer.json
```
