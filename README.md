# install-kind action  <!-- omit in toc -->

[![CI](https://github.com/reconcilerio/install-kind-action/actions/workflows/ci.yaml/badge.svg)](https://github.com/reconcilerio/install-kind-action/actions/workflows/ci.yaml)

Install the kind CLI for the requested version. Attempts to fetch pre-built binaries from the GitHub releases page, or builds from source if a build version is not found.

- [Usage](#usage)
- [Community](#community)
  - [Code of Conduct](#code-of-conduct)
  - [Communication](#communication)
  - [Contributing](#contributing)
- [License](#license)

## Usage

See [action.yml](action.yml)

<!-- start usage -->
```yaml
- uses: reconcilerio/install-kind-action@v1
  with:
    # Optional version.
    # The kind version to install. Resolved as a reference from the sigs.kubernetes.io/kind package.
    # Default: 'latest'
    version: ''
```
<!-- end usage -->

**Basic:**

```yaml
steps:
- uses: reconcilerio/install-kind-action@v1
- run: kind create cluster
```

When building from source, an appropriate go toolchain is required. If unsure, favor a more recent toolchain version.

## Community

### Code of Conduct

The reconciler.io projects follow the [Contributor Covenant Code of Conduct](./CODE_OF_CONDUCT.md). In short, be kind and treat others with respect.

### Communication

General discussion and questions about the project can occur either on the Kubernetes Slack [#reconcilerio](https://kubernetes.slack.com/archives/C07J5G9NDHR) channel, or in the project's [GitHub discussions](https://github.com/orgs/reconcilerio/discussions). Use the channel you find most comfortable.

### Contributing

The reconciler.io wa8s project team welcomes contributions from the community. A contributor license agreement (CLA) is not required. You own full rights to your contribution and agree to license the work to the community under the Apache License v2.0, via a [Developer Certificate of Origin (DCO)](https://developercertificate.org). For more detailed information, refer to [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Apache License v2.0: see [LICENSE](./LICENSE) for details.
