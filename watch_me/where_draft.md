# RuffのConfigurationについて

## 経過（草稿）
```toml
[tool.ruff]
include = [
    "src/**/*.py",
    "tests/**/*.py",
    "scripts/**/*.py",
    "pyproject.toml",
]
cache-dir = ".dev_cache/.ruff_cache"
line-length = 88
indent-width = 4
target-version = "py315"
```
という普段から使っている設定を書いた。
しかし
