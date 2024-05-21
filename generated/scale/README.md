
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:85fb826bdafff98bac9046001f8fb6e8dd5da67c2322b12b2e436ba86ff3d99a |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:ccb895d8916171352aed2f06d9d6f3a1a7aba20405cd129091e9b57d59ad1343 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:78bd4a9ca171ff062a9de912ea782a7eb1208ec68d04e1e71a12767fed8e8d1c |

## IBM Storage Scale images acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:449c668899792e372dff3af01dddcff8ef33fbee1d74dadec68bb9db893e1782 |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:449c668899792e372dff3af01dddcff8ef33fbee1d74dadec68bb9db893e1782 |
| workerX/masterX* | gpfs (Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:b6845d9b04444a0a770eb8f563e9f4085528b92a9a4dbbd5c41e74632e81c644 |
| workerX/masterX* | gpfs (Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:a52a152b2b0246c29570b6ac0cf47208dad1ecc1eb421dcfce78276b4eab6bae |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:582e18f13291d7c686ec4e6e92d20b24c62ae0fc72767c46f30a69b1a6198055  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:29e828701e55c5de848f83a188b2a09de35227aeb6bbdc06ad01b5ec34d2c654 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:815ee1b6af28e693a9b1d54b2b496a3e7dc5b25c51cf60e17a7faa222e44a8b3 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:582e18f13291d7c686ec4e6e92d20b24c62ae0fc72767c46f30a69b1a6198055 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:e02ff8178625200b8835ef2e7ce6d039cf2ae1a5e1b5c0f97c73a00603d9d79e |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:815ee1b6af28e693a9b1d54b2b496a3e7dc5b25c51cf60e17a7faa222e44a8b3 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:8bf1a89ee1e9e52a3f9cd49e1c1747b02fbe7f84f071667ab0e12ea6f25f32f2 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:a61878203bb642320e67edc9229bf84ad37ef0828522ad6d8566bd7747d631f6 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:85fb826bdafff98bac9046001f8fb6e8dd5da67c2322b12b2e436ba86ff3d99a
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:b6845d9b04444a0a770eb8f563e9f4085528b92a9a4dbbd5c41e74632e81c644
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:a52a152b2b0246c29570b6ac0cf47208dad1ecc1eb421dcfce78276b4eab6bae
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:449c668899792e372dff3af01dddcff8ef33fbee1d74dadec68bb9db893e1782
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:e02ff8178625200b8835ef2e7ce6d039cf2ae1a5e1b5c0f97c73a00603d9d79e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:815ee1b6af28e693a9b1d54b2b496a3e7dc5b25c51cf60e17a7faa222e44a8b3
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:29e828701e55c5de848f83a188b2a09de35227aeb6bbdc06ad01b5ec34d2c654
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:8bf1a89ee1e9e52a3f9cd49e1c1747b02fbe7f84f071667ab0e12ea6f25f32f2
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:78bd4a9ca171ff062a9de912ea782a7eb1208ec68d04e1e71a12767fed8e8d1c
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:582e18f13291d7c686ec4e6e92d20b24c62ae0fc72767c46f30a69b1a6198055
cp.icr.io/cp/spectrum/scale/postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:ccb895d8916171352aed2f06d9d6f3a1a7aba20405cd129091e9b57d59ad1343
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:a61878203bb642320e67edc9229bf84ad37ef0828522ad6d8566bd7747d631f6
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0
```
