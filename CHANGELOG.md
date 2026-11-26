# Changelog

## 1.0.0

**Release date:** TBD

Version 1.0.0 is the first release of `semver`, which runs on Lus 2.0.

- Added the `semver` package.
  - `semver.parse`: Parses a version into a table that compares with `<`, `<=`, and `==`.
  - `semver.valid`: Returns the parsed version, or `nil` for text that is not a valid version.
  - `semver.compare`: Compares two versions and returns `-1`, `0`, or `1`.
  - `semver.increment`: Returns a new version with its major, minor, patch, or prerelease part increased.
  - `semver.range`: Parses a range in the syntax of npm.
  - `semver.satisfies`: Returns true if a version is in a range.
  - `semver.max_satisfying`: Returns the highest version of a list that is in a range.
  - `semver.sort`: Returns a copy of a list of versions sorted from the lowest to the highest.
