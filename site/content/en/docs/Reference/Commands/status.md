---
title: "status"
linkTitle: "status"
weight: 1
date: 2019-08-01
description: >
  Gets the status of a local kubernetes cluster
---


### Overview

Gets the status of a local kubernetes cluster.
	Exit status contains the status of minikube's VM, cluster and kubernetes encoded on it's bits in this order from right to left.
	Eg: 7 meaning: 1 (for minikube NOK) + 2 (for cluster NOK) + 4 (for kubernetes NOK)

### Usage

```
minikube status [flags]
```

### Options

```
      --format string   Go template format string for the status output.  The format for Go templates can be found here: https://golang.org/pkg/text/template/
                        For the list accessible variables for the template, see the struct values here: https://godoc.org/k8s.io/minikube/cmd/minikube/cmd#Status (default "host: {{.Host}}\nkubelet: {{.Kubelet}}\napiserver: {{.APIServer}}\nkubectl: {{.Kubeconfig}}\n")
  -h, --help            help for status
```

### Options inherited from parent commands

```
      --alsologtostderr                  log to standard error as well as files
  -b, --bootstrapper string              The name of the cluster bootstrapper that will set up the kubernetes cluster. (default "kubeadm")
      --log_backtrace_at traceLocation   when logging hits line file:N, emit a stack trace (default :0)
      --log_dir string                   If non-empty, write log files in this directory
      --logtostderr                      log to standard error instead of files
  -p, --profile string                   The name of the minikube VM being used. This can be set to allow having multiple instances of minikube independently. (default "minikube")
      --stderrthreshold severity         logs at or above this threshold go to stderr (default 2)
  -v, --v Level                          log level for V logs
      --vmodule moduleSpec               comma-separated list of pattern=N settings for file-filtered logging
```
