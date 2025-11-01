# Pipelines (WIP)

Centralized repository for Git forges automation components.

It provides reusable CI/CD pipelines, quality checks, and configuration patterns.
Designed to provide security consistency, reduce duplication, and minimize maintenance workload.

## GitHub

### Reusable workflows

| Workflow                       | Description                                    |
|--------------------------------|------------------------------------------------|
| [go-checks][go-checks-uri]     | Go code quality checks.                        |
| [go-deploy][go-deploy-uri]     | Go code build and deployment.                  |
| [secops][secops-uri]           | Security scanning and misconfiguration checks. |
| [semver][semver-uri]           | Semantic versioning and release automation.    |
| [yaml-checks][yaml-checks-uri] | YAML quality checks.                           |

[go-checks-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/go-checks.yaml
[go-deploy-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/go-deploy.yaml
[secops-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/secops.yaml
[semver-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/semver.yaml
[yaml-checks-uri]: https://github.com/ttybitnik/pipelines/blob/master/.github/workflows/yaml-checks.yaml

<!-- ### Reusable actions -->

<!-- | Action           | Description               | -->
<!-- |------------------|---------------------------| -->
<!-- | [name][name-uri] | Brief action description. | -->

<!-- [name-uri]: https://github.com/ttybitnik/pipelines/.github/actions/name/action.yaml -->

## Requirements

None

## Example

### Using `workflows`:

```yaml
```

### Using `actions`:

```yaml
```

## License

GPL-3.0

## Author information

Vinícius Moraes ([ttybitnik](https://github.com/ttybitnik))
