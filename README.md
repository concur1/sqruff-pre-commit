# Sqruff-pre-commit

A [pre-commit](https://pre-commit.com/) hook for [Sqruff](https://github.com/quarylabs/sqruff).

### Using sqruff with pre-commit

To run Ruff's [linter](https://docs.astral.sh/ruff/linter) and [formatter](https://docs.astral.sh/ruff/formatter)
(available as of Ruff v0.0.289) via pre-commit, add the following to your `.pre-commit-config.yaml`:

```yaml
repos:
- repo: https://github.com/concur1/sqruff-pre-commit
  # Ruff version.
  rev: v0.18.0
  hooks:
    # Run the formatter.
    - id: sqruff-fix
    # Run the linter.
    - id: sqruff-lint
```

