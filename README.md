# schemafixer-action

GitHub Action to install [schemafixer](https://github.com/bfv/schemafixer) in your workflow.

## Usage

```yaml
- uses: bfv/schemafixer-action@v1

- name: Run schemafixer
  run: schemafixer --help
```

## Inputs

| Input | Description | Required | Default |
|-------|-------------|----------|---------|
| `version` | Version of schemafixer to install (e.g. `v1.0.2`) | No | `latest` |

## Examples

### Use latest version
```yaml
steps:
  - uses: actions/checkout@v4

  - uses: bfv/schemafixer-action@v1

  - name: Run schemafixer
    run: schemafixer --help
```

### Use specific version
```yaml
steps:
  - uses: actions/checkout@v4

  - uses: bfv/schemafixer-action@v1
    with:
      version: 'v1.0.2'

  - name: Run schemafixer
    run: schemafixer --help
```

## releasefixer
See [github.com/bfv/schemafixer](https://github.com/bfv/schemafixer) for the syntax.

## License

MIT