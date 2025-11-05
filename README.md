# Pipelines

Centralized repository of reusable automation components for Git forges.

It provides reusable CI/CD pipelines, quality checks, and configuration patterns to **enforce security**, **reduce duplication**, and **ease maintenance** across multiple repositories.

[![release](https://img.shields.io/github/v/release/ttybitnik/pipelines)](https://github.com/ttybitnik/pipelines/releases/latest)
[![ci/cd](https://github.com/ttybitnik/pipelines/actions/workflows/cd.yaml/badge.svg)](https://github.com/ttybitnik/pipelines/actions/workflows/cd.yaml)
[![conventional commits](https://img.shields.io/badge/conventional%20commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)

## GitHub

### Reusable workflows

| Workflow                                 | Description                                    |
|------------------------------------------|------------------------------------------------|
| [container-checks][container-checks-uri] | Container quality checks.                      |
| [go-checks][go-checks-uri]               | Go code quality checks.                        |
| [go-deploy][go-deploy-uri]               | Go code build and deployment.                  |
| [secops][secops-uri]                     | Security scanning and misconfiguration checks. |
| [semver][semver-uri]                     | Semantic versioning and release automation.    |
| [yaml-checks][yaml-checks-uri]           | YAML quality checks.                           |

[container-checks-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/container-checks.yaml
[go-checks-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/go-checks.yaml
[go-deploy-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/go-deploy.yaml
[secops-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/secops.yaml
[semver-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/semver.yaml
[yaml-checks-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/yaml-checks.yaml

### Actions

| Action                                                   | Description                              |
|----------------------------------------------------------|------------------------------------------|
| [mkdev-custom][mkdev-custom-uri]                         | Custom linter and update scripts checks. |
| [release-please-draft-tag][release-please-draft-tag-uri] | Git tag for release-please drafts.       |

[mkdev-custom-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/actions/mkdev-custom/action.yaml
[release-please-draft-tag-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/actions/release-please-draft-tag/action.yaml

## Requirements

None

## Examples

> [!NOTE]
> Releases in this repository are immutable. Feel free to use the full semantic version (e.g., `v0.1.2`).

### Using `workflows`:

```yaml
jobs:
  go-checks:
    permissions:
      contents: read
      pull-requests: read
      security-events: write
    uses: ttybitnik/pipelines/.github/workflows/go-checks.yaml@v0.1.0  # x-release-please-version
    with:
      codeql-enable: true

  secops:
    permissions:
      contents: read
      security-events: write
    uses: ttybitnik/pipelines/.github/workflows/secops.yaml@v0.1.0  # x-release-please-version
```

### Using `actions`:

```yaml
jobs:
  release-please-draft-tag:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    steps:
      - name: Checkout default branch
        uses: actions/checkout@08c6903cd8c0fde910a37f88322edcfb5dd907a8  # v5.0.0
        with:
          fetch-depth: "0"
      - name: Create git tag for release-please draft
        id: draft-tag
        uses: ttybitnik/pipelines/.github/actions/release-please-draft-tag@v0.1.0  # x-release-please-version
```

## License

GPL-3.0

## Author information

Vinícius Moraes ([ttybitnik](https://github.com/ttybitnik))
