# install-kind cloud-provider-kind action  <!-- omit in toc -->

Install the cloud-provider-kind CLI for the requested version. Attempts to fetch pre-built binaries from the GitHub releases page, or builds from source if a build version is not found.

## Usage

See [action.yml](action.yml)

<!-- start usage -->
```yaml
- uses: reconcilerio/install-kind-action/cloud-provider-kind@v1
  with:
    # Optional version.
    # The cloud-provider-kind version to install. Resolved as a reference in the sigs.k8s.io/cloud-provider-kind module.
    # Default: 'latest'
    version: ''
```
<!-- end usage -->

**Basic:**

```yaml
steps:
- uses: reconcilerio/install-kind-action/cloud-provider-kind@v1
- run: cloud-provider-kind
```

When building from source, an appropriate go toolchain is required. If unsure, favor a more recent toolchain version.
