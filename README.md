# settings.json
## user
```
{
    // 仮想環境のパス。作成した Anaconda仮想環境を指定する。
    "python.venvPath": "${env:CONDA_ENVS_PATH}/elmspy",
    "python.linting.mypyEnabled": true,
    "python.linting.enabled": true,
    "python.linting.mypyArgs": [
        "--follow-imports=silent",
        "--ignore-missing-imports",
        "--show-column-numbers",
        "--no-pretty",
        "--check-untyped-defs"
    ],
    // リンタの設定
    "python.linting.pylintEnabled": false,
    "python.linting.flake8Enabled": true,
    "python.linting.lintOnSave": true,
    "python.linting.flake8Args": [
        "--max-line-length",
        "88",
        "--ignore=E203,W503,W504"
    ],
    // フォーマッタの設定
    "python.formatting.provider": "black",
    "editor.formatOnSave": true,
    "editor.formatOnPaste": false,
    // Docstring
    "autoDocstring.docstringFormat": "numpy",
    "autoDocstring.startOnNewLine": true,
}
```
## folder
```
{
    "terminal.integrated.defaultProfile.windows": "Command Prompt",
    // 拡張機能のロード時にターミナルでPython環境をアクティブにする。
    "python.terminal.activateEnvInCurrentTerminal": true,
    "python.autoComplete.extraPaths": [
        "${env:CONDA_ENVS_PATH}/archi_patterns/Lib/site-packages",
    ],
    // Pythonコマンドのパス。作成した Anaconda仮想環境配下の python.exe を指定する。
    "python.pythonPath": "${env:CONDA_ENVS_PATH}/archi_patterns/python.exe",
    "python.defaultInterpreterPath": "${env:CONDA_ENVS_PATH}/archi_patterns/python.exe",
    "python.analysis.extraPaths": [
        "${env:CONDA_ENVS_PATH}/archi_patterns/Lib/site-packages"
    ],
}
```
