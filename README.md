# 📢Python-CI-Templates

Python-CI-Template is a template for local code quality checks and CI with GitHub Actions.

## 📍Tool Versions

This template uses the following tool versions:

| Tool | Version |
| --- | --- |
|Python|3.15.*|
| uv | 0.13.* |
|uv_build|0.13.*|

## 📍Commands (Comming Soon)

The `Justfile` provides useful shortcuts for linting, formatting, type checking, testing, and installing Git hooks.

### 📝Example Recipes
```just
ruff-modify: ruff-lint ruff-format

ruff-lint:
    uv run ruff check --fix {{TARGETS}}

ruff-format:
    uv run ruff format {{TARGETS}}
```

## 📍Git Hooks (Comming Soon)

Git hooks are installed using `pre-commit` and configured in `.pre-commit-config.yaml`. The hooks use the settings defined in `pyproject.toml` for `ruff`, `mypy`, and `pytest`.

## 📍GitHub Actions (Comming Soon)

The CI workflow is configured in `ci.yml`. It uses local hooks rather than mirror repositories to keep checks consistent between local development and CI.
