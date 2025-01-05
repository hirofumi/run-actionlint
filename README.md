# run-actionlint

## Usage

```yaml
name: Run actionlint

on:
  pull_request:
  push:
    branches:
      - main

jobs:
  run:
    runs-on: ubuntu-latest
    steps:
      - uses: hirofumi/run-actionlint@v1.7.6
```
