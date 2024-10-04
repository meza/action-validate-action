# Action Validate Action

Validates the workflow and action definition files

## Usage

To use this action, include it in your workflow file. Here is an example:

```yaml
name: Validate Action
on: [push, pull_request]

jobs:
  validate-action:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v4
      - name: Validate Action
        uses: meza/action-validate-action@v1
```
