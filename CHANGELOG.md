# Changelog

## [0.3.0](https://github.com/ttybitnik/pipelines/compare/v0.2.0...v0.3.0) (2025-12-04)


### Features

* **container:** add omni fallback output to summary ([92a5265](https://github.com/ttybitnik/pipelines/commit/92a5265a6754c097f9affa680b183380124a9dda))
* **mkdev:** add omni update fallback step ([1a966b3](https://github.com/ttybitnik/pipelines/commit/1a966b3e3f8ed431dd3332350174de4c21f196d7))


### Dependencies

* **gh:** bump actions/setup-go from 6.0.0 to 6.1.0 ([#8](https://github.com/ttybitnik/pipelines/issues/8)) ([23093c8](https://github.com/ttybitnik/pipelines/commit/23093c817e1c16b61fd10ae05d1d96bbbe0a38f8))
* **gh:** bump actions/setup-python from 6.0.0 to 6.1.0 ([#11](https://github.com/ttybitnik/pipelines/issues/11)) ([83d3664](https://github.com/ttybitnik/pipelines/commit/83d3664cd0cd320ca4dfa58f551e04c1c461ea82))
* **gh:** bump github/codeql-action from 4.31.4 to 4.31.6 ([#12](https://github.com/ttybitnik/pipelines/issues/12)) ([56b7572](https://github.com/ttybitnik/pipelines/commit/56b7572fecfe6afe00fcf39f89df6e9e85257861))
* **gh:** bump golangci/golangci-lint-action from 9.0.0 to 9.1.0 ([#7](https://github.com/ttybitnik/pipelines/issues/7)) ([82c200c](https://github.com/ttybitnik/pipelines/commit/82c200c2c447c0372cd49b8837955ab4b87221f5))

## [0.2.0](https://github.com/ttybitnik/pipelines/compare/v0.1.0...v0.2.0) (2025-11-22)


### Features

* **gh:** add container-checks workflow ([7fdd1fe](https://github.com/ttybitnik/pipelines/commit/7fdd1fe7ce0f007e1f3db1fcc14845400c17855f))
* **gh:** add mkdev-custom action ([c6e8f18](https://github.com/ttybitnik/pipelines/commit/c6e8f18c9db5abfa9f970ff3dc8168aeb8bdf5a8))
* **semver:** define inputs types explicitly ([ac7c554](https://github.com/ttybitnik/pipelines/commit/ac7c554dd45e93b331fee1720c8c92358572ca13))


### Bug Fixes

* **container:** remove duplicate inputs key ([7a88f7d](https://github.com/ttybitnik/pipelines/commit/7a88f7d14091dfc637900631968f097eceadabe6))
* **mkdev:** add missing shell required property ([d8a486f](https://github.com/ttybitnik/pipelines/commit/d8a486f2d76306eef41bc2e1d26915a44727fd6a))


### Dependencies

* **gh:** bump actions/checkout from 5.0.0 to 5.0.1 ([#5](https://github.com/ttybitnik/pipelines/issues/5)) ([e7f83b8](https://github.com/ttybitnik/pipelines/commit/e7f83b8a3f3aee85fba93f088fb67550bf04e149))
* **gh:** bump github/codeql-action from 4.31.2 to 4.31.3 ([#6](https://github.com/ttybitnik/pipelines/issues/6)) ([3be85a0](https://github.com/ttybitnik/pipelines/commit/3be85a09bcecdef5ac8aebdb70bdf88eef392e9e))
* **gh:** bump golangci/golangci-lint-action from 8.0.0 to 9.0.0 ([#4](https://github.com/ttybitnik/pipelines/issues/4)) ([9acd3ac](https://github.com/ttybitnik/pipelines/commit/9acd3ac14a2b52ddf69be301b8808c41b1e6517b))

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
