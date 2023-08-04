# Visual Studio Code Settings

## I. User settings

```json
{
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "One Dark Pro",
  "security.workspace.trust.enabled": false,
  "git.allowForcePush": true,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "cSpell.diagnosticLevel": "Hint",
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "[sql]": {
    "editor.defaultFormatter": "cweijan.vscode-database-client2"
  },
  "scm.showIncomingChanges": "never",
  "scm.showOutgoingChanges": "never",
  "terminal.integrated.profiles.windows": {
    "PowerShell": {
      "source": "PowerShell",
      "icon": "terminal-powershell"
    },
    "Command Prompt": {
      "path": [
        "${env:windir}\\Sysnative\\cmd.exe",
        "${env:windir}\\System32\\cmd.exe"
      ],
      "args": [],
      "icon": "terminal-cmd"
    },
    "Git Bash": {
      "source": "Git Bash"
    },
    "Laragon": {
      "path": "${env:windir}\\System32\\cmd.exe",
      "args": ["/k", "C:\\laragon\\bin\\cmder\\vendor\\init.bat"],
      "icon": "terminal-cmd"
    }
  },
  "terminal.integrated.defaultProfile.windows": "Laragon"
}
```

## II. Language settings

> .vscode/settings.json

### 1. JavaScript

```json
{
  "editor.fontSize": 15,
  "editor.wordWrap": "on",

  "workbench.tree.indent": 15,

  "prettier.tabWidth": 4,
  "prettier.printWidth": 110,
  "prettier.endOfLine": "lf",
  "prettier.semi": true,
  "prettier.singleQuote": false,
  "prettier.bracketSpacing": false,

  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "search.exclude": {
    "**/node_modules": true
  }
}
```

### 2. Python

```json
{
  "editor.fontSize": 15,
  "editor.wordWrap": "on",

  "workbench.tree.indent": 15,

  "prettier.tabWidth": 4,
  "prettier.printWidth": 110,
  "prettier.endOfLine": "lf",
  "prettier.semi": true,
  "prettier.singleQuote": false,
  "prettier.bracketSpacing": false,

  "javascript.validate.enable": false,

  "python.envFile": "${workspaceFolder}/.venv",
  "black-formatter.importStrategy": "fromEnvironment",
  "black-formatter.args": ["--line-length", "110"],
  "[python]": {
    "editor.defaultFormatter": "ms-python.black-formatter"
  },
  "search.exclude": {
    "**/.venv": true,
    "**/.vscode": true
  }
}
```

### 3. Flask

```json
{
  "editor.wordWrap": "on",
  "editor.fontSize": 15,
  "editor.defaultFormatter": "esbenp.prettier-vscode",

  "workbench.tree.indent": 15,

  "prettier.tabWidth": 4,
  "prettier.printWidth": 110,
  "prettier.endOfLine": "lf",
  "prettier.semi": true,
  "prettier.singleQuote": false,
  "prettier.bracketSpacing": false,

  "javascript.validate.enable": false,

  "djlint.useVenv": true,
  "djlint.pythonPath": "python3.10",
  "djlint.ignore": ["H021", "H006"],

  "python.envFile": "${workspaceFolder}/.venv",
  "black-formatter.importStrategy": "fromEnvironment",
  "black-formatter.args": ["--line-length", "100"],

  "[python]": {
    "editor.defaultFormatter": "ms-python.black-formatter"
  },
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/Thumbs.db": true,
    "**/__pycache__": true
  },
  "files.associations": {
    "**/views/**/*.html": "jinja-html"
  },
  "material-icon-theme.files.associations": {
    "*.html": "html"
  },
  "material-icon-theme.folders.associations": {
    "forms": "python",
    "storage": "database"
  },
  "emmet.includeLanguages": {
    "jinja-html": "html"
  },
  "[jinja-html]": {
    "editor.defaultFormatter": "monosans.djlint"
  },
  "search.exclude": {
    "**/.venv": true,
    "**/.vscode": true
  }
}
```
