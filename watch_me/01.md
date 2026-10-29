# Settings(Top-level)

## bultins
通常の組み込み関数（`len`や`print`)・・・

## cache-dir
キャッシュディレクトリのパス。

1. ユーザ設定値
2. 環境変数(RUFF_CACHE_DIR)
3. デフォルト設定値
の順で優先される。

本プロジェクトでは`".dev_cache/.ruff_cache"`を採用。

## exclude

本プロジェクトではデフォルト値を尊重して書き換えない。
除外対象を追加する必要がある場合は、`extend-exclude`を参照。

## extend

本プロジェクトでは、デフォルト値を書き換えない。`./pyproject.toml`に設定を集約してあるためである。

## extend-exclude

本プロジェクトでは、デフォルト値を書き換えない。

## extend-include

本プロジェクトでは、デフォルト値を書き換えない。

## extention

本プロジェクトでは、デフォルト値を書き換えない。

## fix

本プロジェクトでは、デフォルト値を書き換えない。コマンドが紛らわしくなり、テンプレートとして不適当だから。

## fix-only

本プロジェクトでは、デフォルト値を書き換えない。同様に、コマンドが紛らわしくなるから。

## force-exclude

公式では`ruff-pre-commit`を使うケースでは、`true`が推奨される。

本プロジェクトでは、デフォルト値を書き換えない。

## include

> [!IMPORTANT]
> 本プロジェクトでは、初学者向けに、設定を書き換えた。以下を参照。

プロジェクトがsrcレイアウトだと仮定。
*.pyファイルだけを対象として、ipynbやmdは対象外とした。
srcディレクトリとtestディレクトリを追加し、
利便性を考慮して、scriptsディレクトリも対象とした。
設定ファイルとして./pyproject.tomlにだけを参照するようにした。

## output-prefer-rule-codes

本プロジェクトでは、初学者向けとして`true`を採用。

## list

| Default value   | Type  | Project                     |
| --------------- | ----- | --------------------------- |
| `".ruff_cache"` | `str` | `".dev_cache/.ruff_cache/"` |
