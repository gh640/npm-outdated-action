# `npm-outdated-action`

A composite action for GitHub Actions that runs `npm outdated --json` and prints the result to summary.

## Prerequisites

- `npm` v8 / v7

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

### Inputs

| name | description |
| --- | --- |
| `cwd` | working directory |

### Outputs

| name | description |
| --- | --- |
| `exitCode` | exit code of the command |
| `stdout` | standard output of the command |
| `stderr` | standard error of the command |

## Sample screenshots

![screenshot](./assets/screenshot.png)

