
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:d44f11cc61f410dd20d7bb52ac28eebc80f928eede9be434c270a7ad5648b626 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:bd264199ac10d574163bfa32bb88844fd786ee6f794a56e235591d2f051c7807 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:eab5b2e72579b96f2cfc04162e4dd6ace7eb3570f2f08dca552c045ea29faa3d |
{: caption="Images (non-entitled)" caption-side="bottom"}

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:089718b2d96d909b86bf19448c4d86f31a3877eb450d465d830e55133415015d |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:089718b2d96d909b86bf19448c4d86f31a3877eb450d465d830e55133415015d |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:0a6c1c0c588168bde48c82ae0ab2ad0ab51429680840dca90f19b24fcbfc3c2c |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:65a1b65e4076ac7be840904a6a1d59eb74849cda58a1a4a59b2f9a8de94652de |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:bc552efb4966aaa44b02532be3168ac1ff18e2af299d0fe89502a1d9fabafbc5  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:93288c812f0bace075eb785f519d6d7f684bdb33407c44a93b53df9abdd16e0a |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:3f41d20e7beaf757778d8650172adf8456569607dab3479eb4524407ed2e4a13 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:bc552efb4966aaa44b02532be3168ac1ff18e2af299d0fe89502a1d9fabafbc5 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:07a9e951ab315724ca39e332a7559ca98519442b0669241fd97ffdb3a0381667 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:3f41d20e7beaf757778d8650172adf8456569607dab3479eb4524407ed2e4a13 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:1a29ab1e4ecdc33a84062cec757620d9787c28b28793202c5b78ae097c3dee27  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:d69cc72025f7c40dae112ff989e920a3331583497c8dfb1600c5ae0e37184a29 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:de79c8bbc271622eb94d2ee8689f189ea7c1cb6adac260a421980fe5eed66708 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987 |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:c53535af8a7f7e3164609838c4b191b42b2d81238d75c1b2a2b582ada62a9780 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:4c148bbdf883153bc72d321be4dc55c33774a6d98b2b3e0c2da6ae389149a9b7 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:b2bc343eadbc11d9ed74a8477d2cd0a7a8460a72203d3f6236d4662e68df1166 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:a6ca689d8205f17bb278910c521842f98ced8537aba55b287792a91269bf2f41 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e |
{: caption="Images (entitled)" caption-side="bottom"}

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:d44f11cc61f410dd20d7bb52ac28eebc80f928eede9be434c270a7ad5648b626
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:0a6c1c0c588168bde48c82ae0ab2ad0ab51429680840dca90f19b24fcbfc3c2c
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:65a1b65e4076ac7be840904a6a1d59eb74849cda58a1a4a59b2f9a8de94652de
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:089718b2d96d909b86bf19448c4d86f31a3877eb450d465d830e55133415015d
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:07a9e951ab315724ca39e332a7559ca98519442b0669241fd97ffdb3a0381667
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:3f41d20e7beaf757778d8650172adf8456569607dab3479eb4524407ed2e4a13
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:93288c812f0bace075eb785f519d6d7f684bdb33407c44a93b53df9abdd16e0a
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:a6ca689d8205f17bb278910c521842f98ced8537aba55b287792a91269bf2f41
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:eab5b2e72579b96f2cfc04162e4dd6ace7eb3570f2f08dca552c045ea29faa3d
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:bc552efb4966aaa44b02532be3168ac1ff18e2af299d0fe89502a1d9fabafbc5
cp.icr.io/cp/spectrum/scale/postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:bd264199ac10d574163bfa32bb88844fd786ee6f794a56e235591d2f051c7807
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:b2bc343eadbc11d9ed74a8477d2cd0a7a8460a72203d3f6236d4662e68df1166
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:1a29ab1e4ecdc33a84062cec757620d9787c28b28793202c5b78ae097c3dee27
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:de79c8bbc271622eb94d2ee8689f189ea7c1cb6adac260a421980fe5eed66708
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:c53535af8a7f7e3164609838c4b191b42b2d81238d75c1b2a2b582ada62a9780
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:d69cc72025f7c40dae112ff989e920a3331583497c8dfb1600c5ae0e37184a29
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:4c148bbdf883153bc72d321be4dc55c33774a6d98b2b3e0c2da6ae389149a9b7
```

