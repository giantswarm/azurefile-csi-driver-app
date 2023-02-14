# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project's packages adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

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

[Unreleased]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v1.20.0-gs1...HEAD
[1.20.0-gs1]: https://github.com/giantswarm/azurefile-csi-driver-app/compare/v0.0.0...v1.20.0-gs1
