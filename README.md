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
        uses: <your-github-username>/publish-vscode-extension@v1
        with:
          vscode-marketplace-pat: ${{ secrets.VSCODE_MARKETPLACE_PAT }}
```