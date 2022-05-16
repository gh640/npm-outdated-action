# `npm-outdated-action`

A composite action for GitHub Actions that runs `npm outdated --json` and print the result to summary.

## Usage

```yaml
uses: gh640/npm-outdated-action@v1
```

With `cwd` set:

```yaml
uses: gh640/npm-outdated-action@v1
with:
  cwd: ./src
```
