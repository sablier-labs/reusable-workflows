# Github Actions Utils

Reusable GitHub Actions utilities for Sablier projects.

## Actions

| Name                                          | Description        |
| --------------------------------------------- | ------------------ |
| [cache](.github/actions/evm-cache/action.yml) | Cache EVM projects |

## Workflows

### EVM

| Name                                                     | Description                                                |
| -------------------------------------------------------- | ---------------------------------------------------------- |
| [bulloak-check](.github/workflows/bulloak-check.yml)     | Check with Bulloak that Solidity tests conform to BTT spec |
| [evm-lint](.github/workflows/evm-lint.yml)               | Lint an EVM project                                        |
| [forge-build](.github/workflows/forge-build.yml)         | Build a Forge project                                      |
| [forge-coverage](.github/workflows/forge-coverage.yml)   | Measure test coverage for a Forge project                  |
| [forge-test](.github/workflows/forge-test.yml)           | Test a Forge project                                       |
| [slither-analyze](.github/workflows/slither-analyze.yml) | Analyze an Ethereum project with Slither                   |

### Other

| Name                                          | Description                            |
| --------------------------------------------- | -------------------------------------- |
| [cron-stale](.github/workflows/cron-tale.yml) | Cron job to close stale issues and PRs |

## Notes

- The utilities are opinionated and may not fit your needs. For example, we use Bun for managing Node.js dependencies
  and running scripts.
- Several workflows require the smart contract artifacts and the node modules to be cached before running. The
  `forge-build` workflow handles this automatically. You may need to run `forge-build` before, for example,
  `forge-coverage`.

## References

- [Reusing workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
- [Sharing actions and workflows with your organization](https://docs.github.com/en/actions/creating-actions/sharing-actions-and-workflows-with-your-organization)
- [How to start using reusable workflows with GitHub Actions](https://github.blog/2022-02-10-using-reusable-workflows-github-actions/)

## Dependents

A list of dependent repositories.

If we make changes to this repo, we may need to update the CI workflows upstream.

- [sablier-labs/airdrops](https://github.com/sablier-labs/airdrops)
- [sablier-labs/evm-utils](https://github.com/sablier-labs/evm-utils)
- [sablier-labs/flow](https://github.com/sablier-labs/flow)
- [sablier-labs/lockup](https://github.com/sablier-labs/lockup)

## License

This project is licensed under MIT.
