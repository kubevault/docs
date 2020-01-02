---
title: Uninstall Vault CSI Driver
menu:
  docs_{{ .version }}:
    identifier: uninstall-csi-driver
    name: Uninstall
    parent: csi-driver-setup
    weight: 15
menu_name: docs_{{ .version }}
section_menu_id: setup
---

# Uninstall Vault CSI Driver

To uninstall Vault CSI driver, run the following command:

<ul class="nav nav-tabs" id="installerTab" role="tablist">
  <li class="nav-item">
    <a class="nav-link active" id="helm3-tab" data-toggle="tab" href="#helm3" role="tab" aria-controls="helm3" aria-selected="true">Helm 3</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" id="helm2-tab" data-toggle="tab" href="#helm2" role="tab" aria-controls="helm2" aria-selected="false">Helm 2</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" id="script-tab" data-toggle="tab" href="#script" role="tab" aria-controls="script" aria-selected="false">YAML</a>
  </li>
</ul>
<div class="tab-content" id="installerTabContent">
  <div class="tab-pane fade" id="helm3" role="tabpanel" aria-labelledby="helm3-tab">

## Using Helm 3

In Helm 3, release names are [scoped to a namespace](https://v3.helm.sh/docs/faq/#release-names-are-now-scoped-to-the-namespace). So, provide the namespace you used to install the CSI driver when installing.

```console
$ helm uninstall csi-vault --namespace kube-system
```

</div>
<div class="tab-pane fade" id="helm2" role="tabpanel" aria-labelledby="helm2-tab">

## Using Helm 2

```console
$ helm delete csi-vault
```

</div>
<div class="tab-pane fade show active" id="script" role="tabpanel" aria-labelledby="script-tab">

## Using YAML (with Helm 3)

If you prefer to not use Helm, you can generate YAMLs from Vault CSI driver chart and uninstall using `kubectl`.

```console
$ helm template vault-operator appscode/csi-vault --namespace kube-system | kubectl delete -f -
```

</div>
</div>
