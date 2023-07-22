# Home Assistant Andrews & Arnold Quota Integration

[![GitHub Release][releases-shield]][releases]
[![GitHub Activity][commits-shield]][commits]
[![License][license-shield]](LICENSE)

[![hacs][hacsbadge]][hacs]

[![Community Forum][forum-shield]][forum]

_Integration to get broadband quota from Andrews & Arnold._

**This integration will set up the following platforms.**

Platform | Description
-- | --
`sensor` | Show info from Andrews & Arnold Quota API.

## Sensors

| Sensor      | Description                                                                                                                                                                                                               |
| :------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `andrews_arnold_monthly_quota`    | Monthly Quota                                                                                                                                                                                              |
| `sensor.andrews_arnold_quota_remaining` | Monthly Quota Remaining                                                                                                                                                         |
| `sensor.andrews_arnold_quota_status`     | Quota Status |

## Installation

1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
1. If you do not have a `custom_components` directory (folder) there, you need to create it.
1. In the `custom_components` directory (folder) create a new folder called `andrews_arnold_quota`.
1. Download _all_ the files from the `custom_components/andrews_arnold_quota/` directory (folder) in this repository.
1. Place the files you downloaded in the new directory (folder) you created.
1. Restart Home Assistant
1. In the HA UI go to "Configuration" -> "Integrations" click "+" and search for "Andrews & Arnold Quota"

## Installation

### HACS

1. Make sure the [HACS](https://github.com/custom-components/hacs) component is installed and working.
1. Add the project repository `https://github.com/andrew-codechimp/HA-Andrews-Arnold-Quota` as a custom repository to HACS, see: https://hacs.xyz/docs/faq/custom_repositories
1. Search for `Andrews & Arnold Quota` in HACS and install it under the "Integrations" category.

### Manual Installation

<details>
<summary>Show detailed instructions</summary>

Installation via HACS is recommended, but a manual setup is supported.

1. Manually copy custom_component/andrews_arnold_quota folder from latest release to custom_components folder in your config folder.

1. Restart Home Assistant.

</details>

## No Configuration Neccessary

As long as you are connecting via Andrews & Arnold this API will automatically return the quota for the current connection.

Data is refreshed every 30 minutes.

<!---->

## Contributions are welcome!

If you want to contribute to this please read the [Contribution guidelines](CONTRIBUTING.md)

## Disclaimer

This integration is no way approved, endorsed or supported by Andrews & Arnold Ltd

***

[andrews_arnold_quota]: https://github.com/andrew-codechimp/HA-Andrews-Arnold-Quota
[commits-shield]: https://img.shields.io/github/commit-activity/y/andrew-codechimp/HA-Andrews-Arnold-Quota.svg?style=for-the-badge
[commits]: https://github.com/andrew-codechimp/HA-Andrews-Arnold-Quota/commits/main
[hacs]: https://github.com/hacs/integration
[hacsbadge]: https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge
[exampleimg]: example.png
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg?style=for-the-badge
[forum]: https://community.home-assistant.io/
[license-shield]: https://img.shields.io/github/license/andrew-codechimp/HA-Andrews-Arnold-Quota.svg?style=for-the-badge
[releases-shield]: https://img.shields.io/github/release/andrew-codechimp/HA-Andrews-Arnold-Quota.svg?style=for-the-badge
[releases]: https://github.com/andrew-codechimp/HA-Andrews-Arnold-Quota/releases
