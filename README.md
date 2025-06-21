# Sqruff-pre-commit

A [pre-commit](https://pre-commit.com/) hook for [Sqruff](https://github.com/quarylabs/sqruff).

### Using sqruff with pre-commit

To run Sqruff's linter and formatter via pre-commit, add the following to your `.pre-commit-config.yaml`:

```yaml
repos:
- repo: https://github.com/concur1/sqruff-pre-commit
  # Ruff version.
  rev: v0.26.8
  hooks:
    # Run the formatter.
    - id: sqruff-fix
    # Run the linter.
    - id: sqruff-lint
```

