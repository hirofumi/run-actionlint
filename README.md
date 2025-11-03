# run-actionlint

`hirofumi/run-actionlint` is a thin wrapper for `docker://rhysd/actionlint`.
This is a workaround for [dependabot-core#8362](https://github.com/dependabot/dependabot-core/issues/8362).

## Usage

```yaml
name: Run actionlint

on:
  pull_request:
  push:
    branches:
      - main

jobs:
  actionlint:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: hirofumi/run-actionlint@v1.7.8
```
