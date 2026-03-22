# Rook (rook)
Rook is a CNCF graduated cloud-native storage orchestrator for Kubernetes, providing the platform, framework, and support for distributed storage systems to natively integrate with cloud-native environments. It automates the deployment, configuration, provisioning, scaling, upgrading, and monitoring of storage systems, with primary support for Ceph.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/rook/refs/heads/main/apis.yml)

## Scope

- **Type:** Index 
- **Position:** Consuming 
- **Access:** 3rd-Party 

## Tags:

 - Kubernetes, Storage, Cloud Native, Orchestration, Ceph, Graduated

## Timestamps

- **Created:** 2025-01-01 
- **Modified:** 2026-03-18 

## APIs

### Rook Ceph Custom Resource API
Rook extends Kubernetes through Custom Resource Definitions (CRDs) to declaratively manage Ceph storage clusters. The CRD API includes resources for CephCluster, CephBlockPool, CephFilesystem, CephObjectStore, CephObjectStoreUser, and related storage primitives, enabling operators to configure and manage Ceph storage entirely through Kubernetes manifests.

**Human URL:** [https://rook.io/docs/rook/latest/CRDs/Cluster/ceph-cluster-crd/](https://rook.io/docs/rook/latest/CRDs/Cluster/ceph-cluster-crd/)


#### Tags:

 - Kubernetes, CRD, Ceph, Storage, Declarative

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Cluster/ceph-cluster-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/)
- [JSONSchema](json-schema/rook-ceph-cluster-schema.json)

### Rook Ceph Object Storage API
Rook provisions Ceph Object Storage gateways (RGW) that expose an S3-compatible and Swift-compatible object storage API. Applications can interact with Ceph Object Storage using standard S3 API clients, and Rook manages the lifecycle of the object store, buckets, and user credentials through Kubernetes CRDs.

**Human URL:** [https://rook.io/docs/rook/latest/CRDs/Object-Storage/ceph-object-store-crd/](https://rook.io/docs/rook/latest/CRDs/Object-Storage/ceph-object-store-crd/)


#### Tags:

 - Object Storage, S3, Ceph, Swift, Storage

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Object-Storage/ceph-object-store-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/Object-Storage/)
- [OpenAPI](openapi/rook-ceph-object-storage-openapi.yml)
- [JSONSchema](json-schema/rook-ceph-object-store-schema.json)

### Rook Ceph Block Storage API
Rook provides Ceph block storage (RBD) through Kubernetes StorageClasses and PersistentVolumeClaims. The CephBlockPool CRD and associated StorageClass allow applications to dynamically provision block volumes backed by Ceph RADOS Block Device, supporting ReadWriteOnce access modes for stateful workloads.

**Human URL:** [https://rook.io/docs/rook/latest/CRDs/Block-Storage/ceph-block-pool-crd/](https://rook.io/docs/rook/latest/CRDs/Block-Storage/ceph-block-pool-crd/)


#### Tags:

 - Block Storage, Ceph, Kubernetes, PersistentVolume, RBD

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Block-Storage/ceph-block-pool-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/Block-Storage/)
- [JSONSchema](json-schema/rook-ceph-block-pool-schema.json)

### Rook Ceph Shared Filesystem API
Rook manages CephFilesystem resources to provision shared POSIX-compliant file storage backed by CephFS. Multiple pods can simultaneously read and write to shared filesystem volumes, making it suitable for workloads requiring ReadWriteMany access, configured through the CephFilesystem CRD and a corresponding StorageClass.

**Human URL:** [https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/ceph-filesystem-crd/](https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/ceph-filesystem-crd/)


#### Tags:

 - File Storage, CephFS, Kubernetes, Shared Filesystem, POSIX

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/ceph-filesystem-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/)
- [JSONSchema](json-schema/rook-ceph-filesystem-schema.json)

## Common Properties

- [JSONSchema](json-schema/rook-ceph-cluster-schema.json)
- [JSONSchema](json-schema/rook-ceph-block-pool-schema.json)
- [JSONSchema](json-schema/rook-ceph-filesystem-schema.json)
- [JSONSchema](json-schema/rook-ceph-object-store-schema.json)
- [JSON-LD](json-ld/rook-context.jsonld)
- [Website](https://rook.io)
- [Documentation](https://rook.io/docs/rook/latest/)
- [Getting Started](https://rook.io/docs/rook/latest/Getting-Started/quickstart/)
- [GitHub Organization](https://github.com/rook)
- [GitHubRepository](https://github.com/rook/rook)
- [Blog](https://blog.rook.io/)
- [Community](https://rook.io/community/)
- [Slack](https://slack.rook.io)
- [Change Log](https://github.com/rook/rook/blob/master/CHANGELOG.md)
- [Security](https://github.com/rook/rook/blob/master/SECURITY.md)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/rook)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
