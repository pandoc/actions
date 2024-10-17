Setup pandoc
============

GitHub Action that will install the specified pandoc version.
Windows-runners are currently not supported.

## Parameters

The action has one optional parameter: `version`. Use it to
install a specific pandoc version such as `2.19` or `2.17.1.1`.
Omitting that parameter will install the latest released version.

## Example steps

```
      - name: Install
        uses: pandoc/actions/setup@v1
        with:
          version: 2.19

      - name: Run pandoc
        run: pandoc --version
```
