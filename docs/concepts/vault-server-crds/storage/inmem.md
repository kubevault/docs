---
title: In Memory | Vault Server Storage
menu:
  docs_{{ .version }}:
    identifier: inmem-storage
    name: In Memory
    parent: storage-vault-server-crds
    weight: 30
menu_name: docs_{{ .version }}
section_menu_id: concepts
---

> New to KubeVault? Please start [here](/docs/concepts/README.md).

# In-Memory

In `In-Memory` backend storage, data will be kept in memory. If the Kubernetes pod on which vault is running is restarted, then all data will be lost. This is useful for development and experimentation, but the use of this backend is highly discouraged in production. Vault documentation for In-Memory storage can be found in [here](https://www.vaultproject.io/docs/configuration/storage/in-memory.html).

```yaml
apiVersion: kubevault.com/v1alpha1
kind: VaultServer
metadata:
  name: vault-with-inmem
  namespace: demo
spec:
  nodes: 1
  version: "0.11.1"
  backend:
    inmem: {}
```

## spec.backend.inmem

To use In-Memory as storage backend in Vault specify `spec.backend.inmem` in [VaultServer](/docs/concepts/vault-server-crds/vaultserver.md) CRD.

```yaml
spec:
  backend:
    inmem: {}
```
