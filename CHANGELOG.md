# Changelog

All notable changes to functional differences between upstream and our own fork will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## [1.7.2-th.1.1.1] - 2026-09-24

### Fixed

- Hide newly-converted write node's properties panel to prevent pop-up spam


## [1.7.2-th.1.1.0] - 2026-09-24

### Added

- Detect optional file extension template key (`ext_field`) and fill using `file_type` value
  https://github.com/shotgunsoftware/tk-nuke-writenode/pull/67
- handler: Exposed `get_node_profile_settings(node)` method
  https://github.com/shotgunsoftware/tk-nuke-writenode/pull/66
- app: Exposed `handler` property
- hook, exposed both as app and handler property, for callbacks
  https://github.com/shotgunsoftware/tk-nuke-writenode/pull/70
  - `post_profile_changed` called when the write node's profile changes.
  - `post_profile_set` called when the write node's profile is set, regardless of whether it changed.

### Fixed

- New Nuke Write nodes now created under Nuke Root node, inline with `TankWriteNodeHandler.get_nodes()`
  https://github.com/shotgunsoftware/tk-nuke-writenode/pull/68


## [1.7.2-th.1.0.1] - 2026-09-23

### Fixed

- Allow for non-SEQ templates i.e. rendering movie files


## [1.7.2-th.1.0.0] - 2026-09-21

### Added

- This CHANGELOG.md
- CI: Auto-release based on version headers in this CHANGELOG.md
