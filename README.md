# :gear: `setup-circleci` ![](https://github.com/lokst/setup-circleci/workflows/Tests/badge.svg)
> An action that installs the CircleCI CLI on GitHub Actions runners

## About
This action sets up the CircleCI CLI, [`circleci`](https://github.com/CircleCI-Public/circleci-cli), on GitHub's hosted Actions runners.

This action can be run on `ubuntu-latest`, `windows-latest`, and `macos-latest` GitHub Actions runners, and will install and expose a specified version of the `circleci` CLI on the runner environment.

## Usage

Setup the `circleci` CLI:

```yaml
steps:
- uses: lokst/setup-circleci@v1
```

A specific version of the `circleci` CLI can be installed:

```yaml
steps:
- uses: lokst/setup-circleci@v1
  with:
    version: 0.1.15973
```

## Inputs
The actions supports the following inputs:

- `version`: The version of `circleci` to install, defaulting to `latest`

## License
[MIT](LICENSE).
