# WARNING THIS DOES NOT YET WORk AND IS UNDER ACTIVE DEVELOPMENT

# Sprase Checkout Buildkite Plugin

Sparse checkouts a directory from Github. Based on https://buildkite.com/docs/plugins/writing

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: echo sparse-checkout
    plugins:
      - pragmaplatform/sparse-checkout#v1.0.0:
          paths: ["dir1", "dir2"]
```

## Configuration

### `paths` (Required, list)

List of directory paths to sparse checkout.

## Developing

To run the tests:

```shell
docker-compose run --rm tests
```

## Contributing

1. Fork the repo
2. Make the changes
3. Run the tests
4. Commit and push your changes
5. Send a pull request
