# Changelog

## 2023-07-04
### Added
- Suppression rule for Jackson's `CVE-2023-35116`

### Changed
- Set jacoco version to `0.8.8`. Higher versions are failing when used with graalvm native agent

## 2023-06-21
### Changed
- Upgraded `checkstyle` version to `10.12.0`

## 2023-06-04
### Changed
- Disabled OSS Index analyzer by default

## 2023-05-29
### Added
- JVM arg to enable test logs

## 2023-05-10
### Removed
- [#9](https://github.com/devatherock/gradle-includes/issues/9): Dependency check suppression for Jackson 2.14.2

## 2023-05-09
### Added
- [#10](https://github.com/devatherock/gradle-includes/issues/10): Codenarc plugin config

### Changed
- Moved checkstyle, spotless and dependency check into a separate file, so that projects with custom test tasks can import these checks separately

## 2023-05-08
### Changed
- [#16](https://github.com/devatherock/gradle-includes/issues/16): Renamed `spotlessXmlTargets` property to `spotless.xml.targets`

## 2023-05-07
### Added
- [#8](https://github.com/devatherock/gradle-includes/issues/8): Checkstyle rules to detect unused imports and local variables
- CI pipeline to check the gradle files for formatting
- Spotless config to format xml files
- Toggles to enable and disable spotless formatting

### Changed
- Upgraded Checkstyle to `10.10.0` from `8.41`
- Made checkstyle run after spotless, so that spotless can remove unused imports before checkstyle runs
- Dependency check plugin config to not scan gradle plugin dependencies

## 2023-05-06
### Added
- [#7](https://github.com/devatherock/gradle-includes/issues/7): Spotless config to remove unused imports

## 2023-05-02
### Changed
- Addressed gradle 7 `Entry is a duplicate but no duplicate handling strategy has been set` error in `Copy` task

## 2022-03-19
### Added
- Suppression file for `dependency-check` plugin

## 2022-08-06
### Added
- Kotlin lint config to spotless

## 2022-05-09
### Added
- `integration.gradle` with integration test config

## 2022-05-07
### Changed
- Configured test logging for all test tasks

## 2022-05-05
### Added
- `publish.gradle` to publish jars

## 2021-11-06
### Added
- Configuration for ktlint plugin

## 2021-10-16
### Added
- Configuration for dependency check plugin

## 2021-04-08
### Added
- Checkstyle for basic code style checks

## 2021-04-03
### Added
- Spotless config for Groovy

## 2021-03-31
### Added
- Code to download spotless formatter file

## 2021-03-30
### Added
- Config for spotless

## 2020-11-14
### Added
- Sonar properties required for PR analysis
- Simplified way to specify custom jacoco coverage thresholds

## 2020-11-13
### Added
- `checks.gradle` with jacoco and sonarqube