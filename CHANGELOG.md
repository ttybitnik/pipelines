# Changelog

## [0.1.0](https://github.com/ttybitnik/pipelines/compare/v0.1.0...v0.1.0) (2025-11-04)


### Features

* **go-deploy:** use go.mod for version ([4359253](https://github.com/ttybitnik/pipelines/commit/435925394c05229238e55e2e082ad1baa39c7854))
* **go-reploy:** add goreleaser version and args as inputs ([a988fff](https://github.com/ttybitnik/pipelines/commit/a988fffff68a40012622033a6c6247a18fbf901d))
* **project:** initial commit ([6ffffef](https://github.com/ttybitnik/pipelines/commit/6ffffefce5796ddc25d0f92ca3f8907746af761a))
* **semver:** add outputs and summary for tag creation ([bb06f56](https://github.com/ttybitnik/pipelines/commit/bb06f568657d147e678d14e2209d84977d03ffe6))
* **semver:** add release-please-draft-tag action ([60eccfb](https://github.com/ttybitnik/pipelines/commit/60eccfbb12e878f8eb3984ec0b3cd17dcdc04fd2))
* **semver:** add tag_created output for summary ([145d3ff](https://github.com/ttybitnik/pipelines/commit/145d3ffafb1d7e239dc256e68c9505744d3325a7))


### Bug Fixes

* **go-checks:** adjust input for go version file ([32e1236](https://github.com/ttybitnik/pipelines/commit/32e1236f6d038ea3b36fe708096a2fecdd97f703))
* **go-checks:** adjust steps indentation ([ede6518](https://github.com/ttybitnik/pipelines/commit/ede65188754de5dac223bd33e1a8590a8be6ae7f))
* **semver:** stop github-script execution after setFailed calls ([89a3fbb](https://github.com/ttybitnik/pipelines/commit/89a3fbba1c208f5eebc6c158d7a61a4d63fd7200))
* **semver:** use env vars for github-script inputs ([b8d772b](https://github.com/ttybitnik/pipelines/commit/b8d772b289c3ede25edbba4c052b58df829bd438))


### Code Refactoring

* **ci:** abbreviate workflow names for badge display ([41be478](https://github.com/ttybitnik/pipelines/commit/41be478f417b4612a8921567380c8e196af6445a))
* **ci:** rename cd workflow to ci/cd ([1f016a8](https://github.com/ttybitnik/pipelines/commit/1f016a821d3e5baf560250e2005a3e8996f232c4))
* **semver:** replace logging and process control with core methods ([52d8f6d](https://github.com/ttybitnik/pipelines/commit/52d8f6d1b82498b9ce0f72e942bec06c5164102c))
