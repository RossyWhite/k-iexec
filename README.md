# k-iexec

A plugin to perform `kubectl exec` with interactive selector.
  
## Requirements

- [fzf](https://github.com/junegunn/fzf)

## Installation

```bash
export INSTALL=<yourpath> # anywhere inside $PATH
curl https://raw.githubusercontent.com/RossyWhite/k-iexec/master/kubectl-iexec -o $INSTALL/kubectl-iexec
```

## Usage

```bash
$ kubectl iexec --help

Usage: kubectl iexec [OPTIONS...] <query> -- <command>
OPTIONS:
  -h, --help               Show help for 'kubectl iexec'
  -n, --namespace string   The name of namespace to use
  --context string         The name of kubeconfig context to use
Examples:
  kubectl iexec -n kube-system kube-proxy -- /bin/sh
  kubectl iexec istiod --context my-cluster
```
