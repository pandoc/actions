GitHub Actions for Pandoc
=========================

This repository offers GitHub Actions to facilitate the use of
pandoc on that platform.

## `pandoc/actions/setup`

This actions installs pandoc in the current runner. The `version` parameter
allows to install a specific version. The default is to install the latest
version.

### Example

```
jobs:
  pandoc:
    steps:
      - name: Install pandoc
        uses: pandoc/actions/setup@v1

      - name: Run pandoc
        run: pandoc --version
```
