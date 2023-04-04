# Publish VSCode Extension

Action used for publishing VSCode extension to the marketplace.

## Usage

```yaml
on:
  push:
    branches: [master]

jobs:
  publish:
    runs-on: ubuntu-latest
    steps:
      - name: Publish VSCode Extension
        uses: mrzli-gh-actions/publish-vscode-extension@v1.0.0
        with:
          vscode-marketplace-pat: ${{ secrets.VSCODE_MARKETPLACE_PAT }}
```