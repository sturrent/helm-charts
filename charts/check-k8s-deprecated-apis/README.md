# check-k8s-deprecated-apis

[k8s-check-deprecated-apis](https://github.com/sturrent/k8s-check-deprecated-apis) is a simple script that uses the pluto utility to check for depricated APIs on a Kubernetes cluster.

## TL;DR

```console
$ helm repo add sturrent https://sturrent.github.io/helm-charts
$ helm install my-release sturrent/check-k8s-deprecated-apis
```

## Introduction

This chart deploys a pod using the [check-deprecated-apis](https://hub.docker.com/repository/docker/sturrent/check-deprecated-apis) container image on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.
The pod will run the [k8s-check-deprecated-apis](https://github.com/sturrent/k8s-check-deprecated-apis) script and will output the status of deprecated API objects.

## Prerequisites

- Kubernetes 1.14+
- Helm 3.1.0
- Access to pull public container images from dockerhub

## Installing the Chart

To install the chart with the release name `my-release`:

```console
helm install my-release sturrent/check-k8s-deprecated-apis
```

> **Tip**: List all releases using `helm list`

## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```console
helm delete my-release
```

The command removes all the Kubernetes components associated with the chart and deletes the release.
