# Workflows

| Workflow | Runs on | What it does |
| --- | --- | --- |
| [`config-lint.yml`](config-lint.yml) | Push to `main`, every pull request | Checks every `prefs.txt` line is a `#` note or `<type> <key> <value>` with a type `defaults` accepts (`string`, `bool`, `int` or `data`) and no key repeated. Parses the key bindings property list, the eight `.xccolortheme` property lists and the Xcode 27 theme's JSON. Runs `bash -n` and shellcheck on `apply.sh` |
| [`markdownlint.yml`](markdownlint.yml) | Push to `main`, every pull request | Lints every markdown file against [`.markdownlint.json`](../../.markdownlint.json) |

Both are also runnable manually via `workflow_dispatch` from the Actions tab.
