# pre-commit-pint

Pre commit checks for linting with [pint](https://github.com/cloudflare/pint),
which is a brilliant Prometheus rule linter by Cloudflare.

## Config

It will automatically pick up the default pint config.

This can be used to enable relaxed parsing, which allows parsing k8s manifests directly.

#### .pint.hcl
```hcl
parser {
  relaxed = [ "(.*)" ]
}
```
