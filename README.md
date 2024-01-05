# Reusable Workflows

This repository contains a collection of reusable GitHub Actions workflows.

## Tables

### Ethereum

| Name                                                       | Description                               |
| ---------------------------------------------------------- | ----------------------------------------- |
| [forge-build](./.github/workflows/forge-build.yml)         | Build a Forge project                     |
| [forge-coverage](./.github/workflows/forge-coverage.yml)   | Measure test coverage for a Forge project |
| [forge-lint](./.github/workflows/forge-lint.yml)           | Lint a Forge project                      |
| [forge-test](./.github/workflows/forge-test.yml)           | Test a Forge project                      |
| [slither-analyze](./.github/workflows/slither-analyze.yml) | Analyze an Ethereum project with Slither  |

### Miscellaneous

| Name                                   | Description                |
| -------------------------------------- | -------------------------- |
| [stale](./.github/workflows/stale.yml) | Close stale issues and PRs |

## References

- [Reusing workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
- [Sharing actions and workflows with your organization](https://docs.github.com/en/actions/creating-actions/sharing-actions-and-workflows-with-your-organization)
- [How to start using reusable workflows with GitHub Actions](https://github.blog/2022-02-10-using-reusable-workflows-github-actions/)
