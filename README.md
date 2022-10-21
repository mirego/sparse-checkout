# Sparse Checkout

A simple action to perform a sparse checkout of the repository. 
This is a workaround until the feature is added to the main checkout action (see https://github.com/actions/checkout/pull/680).

## Inputs

### `patterns`

**Required** The pattern for the sparse checkout ([see git documentation](https://git-scm.com/docs/git-sparse-checkout)).

### `branch`

**Required** The branch to checkout.

## Example usage

```yaml
uses: mirego/sparse-checkout@v1
  with:
    patterns: subproject/web subproject/ios
    branch: beta
```
