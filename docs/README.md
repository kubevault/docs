---
title: Welcome | KubeVault
description: Welcome to KubeVault
menu:
  docs_0.1.0:
    identifier: readme-kubevault
    name: Readme
    parent: welcome
    weight: -1
product_name: kubevault
menu_name: docs_0.1.0
section_menu_id: welcome
url: /docs/0.1.0/welcome/
aliases:
  - /docs/0.1.0/
  - /docs/0.1.0/README/
---

# KubeVault

KubeVault by AppsCode is a collection of tools for running HashiCorp [Vault](https://www.vaultproject.io/) on Kubernetes. You can deploy and mange Vault using Vault operator. Using Vault operator, you can deploy Vault for following storage backends:

- [Azure](/docs/concepts/vault-server-crds/storage/azure.md)
- [S3](/docs/concepts/vault-server-crds/storage/s3.md)
- [GCS](/docs/concepts/vault-server-crds/storage/gcs.md)
- [DynamoDB](/docs/concepts/vault-server-crds/storage/dynamodb.md)
- [PosgreSQL](/docs/concepts/vault-server-crds/storage/postgresql.md)
- [MySQL](/docs/concepts/vault-server-crds/storage/mysql.md)
- [Swift](/docs/concepts/vault-server-crds/storage/swift.md)
- [In Memory](/docs/concepts/vault-server-crds/storage/inmem.md)
- [Etcd](/docs/concepts/vault-server-crds/storage/etcd.md)


From here you can learn all about Vault operator's architecture and how to deploy and use Vault operator.

- [Concepts](/docs/concepts/). Concepts explain the CRDs (CustomResourceDefinition) used by Vault operator.

- [Setup](/docs/setup/). Setup contains instructions for installing
  the Vault operator in various cloud providers.

- [Monitoring](/docs/guides/monitoring). Monitoring contains instructions for setup prometheus with Vault server

- [Guides](/docs/guides/). Guides show you how to perform tasks with Vault operator.

- [Reference](/docs/reference/). Detailed exhaustive lists of
command-line options, configuration options, API definitions, and procedures.

We're always looking for help improving our documentation, so please don't hesitate to [file an issue](https://github.com/kubevault/project/issues/new) if you see some problem. Or better yet, submit your own [contributions](/docs/CONTRIBUTING.md) to help
make our docs better.

---

**Vault operator binaries collects anonymous usage statistics to help us learn how the software is being used and how we can improve it. To disable stats collection, run the operator with the flag** `--enable-analytics=false`.

---
