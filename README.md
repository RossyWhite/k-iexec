# k-iexec

A plugin to perform `kubectl exec` with interactive selector.
  
## Requirements

- [fzf](https://github.com/junegunn/fzf)

## Installation

```bash
curl -LO https://raw.githubusercontent.com/RossyWhite/k-iexec/v0.0.2/kubectl-iexec
chmod u+x kubectl-iexec
mv kubectl-iexec /usr/local/bin
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
