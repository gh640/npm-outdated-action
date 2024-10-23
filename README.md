# `npm-outdated-action`

A simple composite action for GitHub Actions that runs `npm outdated --json` and prints the result to summary.

## Prerequisites

- `npm`: v10 / v9 / v8 / v7

## Usage

```yaml
- run: npm ci
- uses: gh640/npm-outdated-action@v1
```

With `cwd` set:

```yaml
- run: npm ci
- uses: gh640/npm-outdated-action@v1
  with:
    cwd: ./src
```

You need to install the packages beforehand to display values of the `current` culumn.

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

