# Visual Studio Code Settings

## I. User settings

```json
{
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "One Dark Pro",
  "workbench.tree.indent": 15,
  "workbench.editor.enablePreview": false,
  "security.workspace.trust.enabled": false,
  "git.allowForcePush": true,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "cSpell.diagnosticLevel": "Hint",
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "editor.linkedEditing": true,
  "editor.fontSize": 15,
  "editor.autoClosingBrackets": "always",
  "explorer.compactFolders": false,
  "diffEditor.ignoreTrimWhitespace": false,
  "update.mode": "none",
  "extensions.autoUpdate": false,
  "[sql]": {
    "editor.defaultFormatter": "cweijan.vscode-database-client2"
  },
  "terminal.integrated.profiles.windows": {
    "Cmder": {
      "path": "${env:windir}\\System32\\cmd.exe",
      "args": [
        "/k",
        "${env:USERPROFILE}\\laragon\\bin\\cmder\\vendor\\init.bat"
      ],
      "icon": "terminal-cmd"
    }
  },
  "terminal.integrated.defaultProfile.windows": "cmder",
  "[mjml]": {
    "editor.defaultFormatter": "attilabuti.vscode-mjml"
  },
  "gitlens.graph.layout": "editor",
  "material-icon-theme.activeIconPack": "react_redux",
  "path-intellisense.mappings": {
    "@": "${workspaceFolder}/src"
  },
  "svg.preview.mode": "img",
  "explorer.copyRelativePathSeparator": "/",
  "workbench.tree.enableStickyScroll": false,
  "editor.stickyScroll.scrollWithEditor": false,
  "editor.stickyScroll.enabled": false,
  "[svg]": {
    "editor.defaultFormatter": "jock.svg"
  }
}
```

## II. Language settings

> .vscode/settings.json

### 1. Python

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

### 2. Flask

```json
{
  "editor.formatOnSave": true,
  "editor.wordWrap": "on",
  "editor.fontSize": 15,

  "workbench.tree.indent": 15,

  "javascript.validate.enable": false,

  "djlint.useVenv": true,
  "djlint.pythonPath": "python",

  "python.envFile": "${workspaceFolder}/.venv",
  "python.languageServer": "Pylance",
  "python.analysis.autoImportCompletions": true,
  "black-formatter.importStrategy": "fromEnvironment",

  "[python]": {
    "editor.defaultFormatter": "ms-python.black-formatter",
    "editor.formatOnSave": false
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
    "editor.defaultFormatter": "monosans.djlint",
    "editor.wordWrap": "off"
  },
  "search.exclude": {
    "**/.venv": true,
    "**/.vscode": true,
    "**/static": true
  },
  "terminal.integrated.defaultProfile.windows": "Command Prompt"
}
```
