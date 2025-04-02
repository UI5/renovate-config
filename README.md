![UI5 logo](./docs/images/UI5_logo_wide.png)

# UI5 Renovate Preset

> A Renovate preset to keep your UI5 application up-to-date.

[![OpenUI5 Community Slack (#tooling channel)](https://img.shields.io/badge/slack-join-44cc11.svg)](https://ui5-slack-invite.cfapps.eu10.hana.ondemand.com/)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.1%20adopted-ff69b4.svg)](https://github.com/UI5/renovate-config?tab=coc-ov-file#readme)
[![REUSE status](https://api.reuse.software/badge/github.com/UI5/renovate-config)](https://api.reuse.software/info/github.com/UI5/renovate-config)

- [UI5 Renovate Preset](#ui5-renovate-config)
	- [Features](#features)
	- [Usage](#usage)
	- [Sample](#sample)
	- [Further Information](#further-information)
	- [Support, Feedback, Contributing](#support-feedback-contributing)
	- [Security / Disclosure](#security--disclosure)
	- [Code of Conduct](#code-of-conduct)
	- [Licensing](#licensing)

## Features

Automatically creates pull requests to your UI5 project whenever a new UI5 version is released.

Information on the currently used UI5 version is updated in the following files:
- ui5.yaml files
- HTML files

The UI5 Renovate Preset takes into account whether your project uses [OpenUI5](https://sdk.openui5.org/) or [SAPUI5](https://ui5.sap.com/).

## Usage

1. Set up [Renovate](https://docs.renovatebot.com/getting-started/installing-onboarding/) for your repository.
2. Create a new file called `renovate.json` at the root level of your project.
3. Add the following content:

```json
{
	"$schema": "https://docs.renovatebot.com/renovate-schema.json",
	"extends": [
		"UI5/renovate-config"
	],
	"separateMinorPatch": true
}
```

**Note:** We recommend setting `separateMinorPatch` to `true` to create separate pull requests for patches and minor releases.

If your project should only consume Long-Term Support (LTS) releases, use the following content:

```json
{
	"$schema": "https://docs.renovatebot.com/renovate-schema.json",
	"extends": [
		"UI5/renovate-config:lts"
	],
	"separateMinorPatch": true
}
```

## Sample

See https://github.com/SAP/openui5-sample-app for a live demo of `UI5 Renovate Preset`.

## Further Information

- [Renovate Docs](https://docs.renovatebot.com/)

## Support, Feedback, Contributing

This project is open to feature requests/suggestions, bug reports, etc. via [GitHub issues](https://github.com/UI5/renovate-config/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project's structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).

You can also chat with us in the [`#renovate-config`](https://openui5.slack.com/archives/C0A7QFN6B) channel of the [OpenUI5 Community Slack](https://ui5-slack-invite.cfapps.eu10.hana.ondemand.com/). For public Q&A, use the [`ui5-renovate-config` tag on Stack Overflow](https://stackoverflow.com/questions/tagged/ui5-tooling).

## Security / Disclosure

If you find any bug that might be a security problem, please follow the instructions given in [Security Policy](https://github.com/UI5/renovate-config/security/policy) on how to report it. Please do not create GitHub issues for security-related concerns or problems.

## Code of Conduct

We as members, contributors, and leaders pledge to make participation in our community a harassment-free experience for everyone. By participating in this project, you agree to abide by its [Code of Conduct](https://github.com/UI5/renovate-config?tab=coc-ov-file#readme) at all times.

## Licensing

Copyright 2024 SAP SE or an SAP-affiliate company and contributors. Please see our [LICENSE](./LICENSE) for copyright and license information. Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/UI5/renovate-config).
