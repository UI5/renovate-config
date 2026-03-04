# Changelog

## [1.2.1](https://github.com/UI5/renovate-config/compare/v1.2.0...v1.2.1) (2026-03-04)


### Bug Fixes

* **datasources.json:** Use UI5 GitHub organization for links to source code ([8bdaf6d](https://github.com/UI5/renovate-config/commit/8bdaf6de8126c62a1678f8ba4a62555ce47c699b))

## [1.2.0](https://github.com/UI5/renovate-config/compare/v1.1.1...v1.2.0) (2026-03-03)


### Features

* Migrate 'fileMatch' to 'managerFilePatterns' property ([e22baac](https://github.com/UI5/renovate-config/commit/e22baacebee03f356e7764af92a0d69c3a6326fd))

## [1.1.1](https://github.com/UI5/renovate-config/compare/v1.1.0...v1.1.1) (2025-04-17)


### Bug Fixes

* **openui5_lts:** Result when determining LTS releases is aligned with Renovate schema ([#22](https://github.com/UI5/renovate-config/issues/22)) ([b6dde8d](https://github.com/UI5/renovate-config/commit/b6dde8d30b4c2764680c4c867dbeb2ed332efeca))

## [1.1.0](https://github.com/UI5/renovate-config/compare/v1.0.0...v1.1.0) (2025-04-16)


### Features

* **sapui5:** Upgrade UI5 version maintained in manifest.json or CommonDataModel.json ([#20](https://github.com/UI5/renovate-config/issues/20)) ([6c877cf](https://github.com/UI5/renovate-config/commit/6c877cf54e3b9744198b09df447c42ed895ff3b3)), closes [#15](https://github.com/UI5/renovate-config/issues/15)

## [1.0.0](https://github.com/UI5/renovate-config/compare/v0.0.1...v1.0.0) (2025-04-08)

### General

Automatically creates pull requests to your UI5 project whenever a new UI5 version is released.

Information on the currently used UI5 version is updated in the following files:
* ui5.yaml files
* HTML files

The UI5 Renovate Preset Config also takes into account whether your project uses OpenUI5 or SAPUI5.
