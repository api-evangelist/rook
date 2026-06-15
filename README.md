# Rook (rook)

Rook is a CNCF graduated cloud-native storage orchestrator for Kubernetes, providing the platform, framework, and support for Ceph distributed storage systems to natively integrate with cloud-native environments. It automates the deployment, configuration, provisioning, scaling, upgrading, and monitoring of storage systems through Kubernetes operators and Custom Resource Definitions (CRDs), with primary support for Ceph block storage, shared filesystems, and S3-compatible object storage.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/rook/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/rook/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Block Storage
- CNCF
- Ceph
- Cloud Native
- File Storage
- Graduated
- Kubernetes
- Object Storage
- Orchestration
- Storage

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-05-19

## APIs

### Rook Ceph Custom Resource API

Rook extends Kubernetes through Custom Resource Definitions (CRDs) to declaratively manage Ceph storage clusters. The CRD API includes resources for CephCluster, CephBlockPool, CephFilesystem, CephObjectStore, CephObjectStoreUser, CephNFS, CephRBDMirror, and related storage primitives, enabling operators to configure and manage Ceph storage entirely through Kubernetes manifests.

- **Human URL:** [https://rook.io/docs/rook/latest/CRDs/Cluster/ceph-cluster-crd/](https://rook.io/docs/rook/latest/CRDs/Cluster/ceph-cluster-crd/)

#### Tags

- Ceph
- CRD
- Declarative
- Kubernetes
- Storage

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Cluster/ceph-cluster-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/)
- [JSON Schema](json-schema/rook-ceph-cluster-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/rook-ceph-cluster-structure.json)
- [Postman Collection](collections/rook-ceph-object-storage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rook-ceph-object-storage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Rook Ceph Object Storage API

Rook provisions Ceph Object Storage gateways (RGW) that expose an S3-compatible and Swift-compatible object storage API. Applications can interact with Ceph Object Storage using standard S3 API clients, and Rook manages the lifecycle of the object store, buckets, and user credentials through Kubernetes CRDs.

- **Human URL:** [https://rook.io/docs/rook/latest/CRDs/Object-Storage/ceph-object-store-crd/](https://rook.io/docs/rook/latest/CRDs/Object-Storage/ceph-object-store-crd/)

#### Tags

- Ceph
- Object Storage
- S3
- Storage
- Swift

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Object-Storage/ceph-object-store-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/Object-Storage/)
- [OpenAPI](openapi/rook-ceph-object-storage-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/rook-ceph-object-storage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rook-ceph-object-storage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/rook-ceph-object-store-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/rook-ceph-object-store-structure.json)

### Rook Ceph Block Storage API

Rook provides Ceph block storage (RBD) through Kubernetes StorageClasses and PersistentVolumeClaims. The CephBlockPool CRD and associated StorageClass allow applications to dynamically provision block volumes backed by Ceph RADOS Block Device, supporting ReadWriteOnce access modes for stateful workloads.

- **Human URL:** [https://rook.io/docs/rook/latest/CRDs/Block-Storage/ceph-block-pool-crd/](https://rook.io/docs/rook/latest/CRDs/Block-Storage/ceph-block-pool-crd/)

#### Tags

- Block Storage
- Ceph
- Kubernetes
- PersistentVolume
- RBD

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Block-Storage/ceph-block-pool-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/Block-Storage/)
- [JSON Schema](json-schema/rook-ceph-block-pool-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/rook-ceph-block-pool-structure.json)
- [Postman Collection](collections/rook-ceph-object-storage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rook-ceph-object-storage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Rook Ceph Shared Filesystem API

Rook manages CephFilesystem resources to provision shared POSIX-compliant file storage backed by CephFS. Multiple pods can simultaneously read and write to shared filesystem volumes, making it suitable for workloads requiring ReadWriteMany access, configured through the CephFilesystem CRD and a corresponding StorageClass.

- **Human URL:** [https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/ceph-filesystem-crd/](https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/ceph-filesystem-crd/)

#### Tags

- CephFS
- File Storage
- Kubernetes
- POSIX
- Shared Filesystem

#### Properties

- [Documentation](https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/ceph-filesystem-crd/)
- [Reference](https://rook.io/docs/rook/latest/CRDs/Shared-Filesystem/)
- [JSON Schema](json-schema/rook-ceph-filesystem-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/rook-ceph-filesystem-structure.json)
- [Postman Collection](collections/rook-ceph-object-storage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rook-ceph-object-storage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/rook-security)
- [JSON Schema](json-schema/rook-ceph-cluster-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/rook-ceph-block-pool-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/rook-ceph-filesystem-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/rook-ceph-object-store-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/rook-ceph-cluster-structure.json)
- [JSON-LD](json-ld/rook-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/rook-vocabulary.yml)
- [Rules](rules/rook-spectral-rules.yml)
- [Capabilities](capabilities/storage-orchestration.yaml)
- [Website](https://rook.io)
- [Documentation](https://rook.io/docs/rook/latest/)
- [Getting Started](https://rook.io/docs/rook/latest/Getting-Started/quickstart/)
- [GitHub Organization](https://github.com/rook)
- [GitHub Repository](https://github.com/rook/rook)
- [Blog](https://blog.rook.io/)
- [Community](https://rook.io/community/)
- [Slack](https://slack.rook.io)
- [Changelog](https://github.com/rook/rook/blob/master/CHANGELOG.md)
- [Security](https://github.com/rook/rook/blob/master/SECURITY.md)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/rook)
- [X (Twitter)](https://twitter.com/rook_io)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
