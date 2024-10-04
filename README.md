# sqruff-pre-commit

[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/quarylabs/sqruff)
[![image](https://img.shields.io/pypi/v/sqruff/0.18.0.svg)](https://pypi.python.org/pypi/sqruff)
[![image](https://img.shields.io/pypi/l/sqruff/0.18.0.svg)](https://pypi.python.org/pypi/sqruff)
[![image](https://img.shields.io/pypi/pyversions/sqruff/0.18.0.svg)](https://pypi.python.org/pypi/sqruff)

A [pre-commit](https://pre-commit.com/) hook for [Ruff](https://github.com/quarylabs/sqruff).

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

