# Change log

All notable changes to the LaunchDarkly Node.js SDK will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org).

## [3.0.2] - 2016-08-19
- Fixed a bug in the secure_mode_hash function

## [3.0.1] - 2016-08-18
### Changed
- The `ready` event now gets properly emitted in offline mode.

## [3.0.0] - 2016-08-08
### Added
- Support for multivariate feature flags. In addition to booleans, feature flags can now return numbers, strings, dictionaries, or arrays via the `variation` method.
- New `all_flags` method returns all flag values for a specified user.
- New `secure_mode_hash` function computes a hash suitable for the new LaunchDarkly JavaScript client's secure mode feature.
- New `initialized` function returns whether or not the client has finished initialization.

### Deprecated
- The `toggle` call has been deprecated in favor of `variation`.
