# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project's packages adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed

- Update component versions (sync with upstream chart)
  - `azurefile-csi` to `v1.30.2`
  - `csi-provisioner` to `v4.0.1`
  - `csi-attacher` to `v4.6.1`
  - `csi-resizer` to `v1.10.1`
  - `livenessprobe` to `v2.12.0`
  - `csi-node-driver-registrar` to `v2.10.1`

## [1.26.0-gs5] - 2024-04-15

### Added

- Add `af-premium-private` and `af-standard-private` storage classes using private endpoints to connect to the storage account.

## [1.26.0-gs4] - 2024-01-23

### Changed

- Configure `gsoci.azurecr.io` as the default container image registry.
- Add `imagePullPolicy` to containers that didn't have it.

## [1.26.0-gs3] - 2023-12-14

### Added

- Add team label in resources.
- Add `global.podSecurityStandards.enforced` value for PSS migration.
- Add storage classes for CAPZ.

## [1.26.0-gs2] - 2023-05-03

### Changed

- Disable PSPs for k8s 1.25 and newer.

## [1.26.0-gs1] - 2023-02-14

### Changed

* Sync with upstream 1.26.0 chart
* bump components versions
  * azurefile-csi to `1.26.0`
  * csi-provisioner to `3.3.0`
  * csi-attacher to `4.0.0`
  * csi-resizer to `1.6.0`
  * livenessprobe to `2.8.0`
  * csi-node-driver-registrar to `2.6.2`
* increase api qps limit of csi-provisioner and csi-attacher 
* increase api qps for azurefile kubeclient
* add support for labels, annotations, podLabels and podAnnotations 
* Remove `list` rbac for secrets
* add node-role.kubernetes.io/control-plane toleration
* add support for http/s proxy 
* Make `AZURE_CREDENTIAL_FILE` depends on `.Values.provider`

## [1.20.0-gs1] - 2022-08-29

### Added

- Initial release with upstream version 1.20.

[Unreleased]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v1.26.0-gs5...HEAD
[1.26.0-gs5]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v1.26.0-gs4...v1.26.0-gs5
[1.26.0-gs4]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v1.26.0-gs3...v1.26.0-gs4
[1.26.0-gs3]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v1.26.0-gs2...v1.26.0-gs3
[1.26.0-gs2]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v1.26.0-gs1...v1.26.0-gs2
[1.26.0-gs1]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v1.20.0-gs1...v1.26.0-gs1
[1.20.0-gs1]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v0.0.0...v1.20.0-gs1
