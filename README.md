# protolint-action

![Build Status](https://github.com/plexsystems/protolint-action/workflows/build-test/badge.svg)

A GitHub Action for using [protolint](https://github.com/yoheimuta/protolint) in your [GitHub Action](https://github.com/features/actions) workflows.

## Example

```yaml
name: "lint protobuf"
on: pull_request

jobs:
  pr-check:
    runs-on: ubuntu-latest
    steps:
    - name: checkout source
      uses: actions/checkout@v1

    - name: run protolint
      uses: ssilve1989/protolint-action@v0.1-alpha
```
