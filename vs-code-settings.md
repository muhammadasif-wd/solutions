{
  // editor
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontSize": 16,
  "editor.fontLigatures": true,
  "editor.wordWrap": "on",
  "editor.minimap.enabled": false,
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": [
          "comment",
          "keyword",
          "keyword.control",
          "entity.name.function",
          "entity.name.tag.css",
          "meta.function"
        ],
        "settings": {
          "fontStyle": "italic"
        }
      }
    ]
  },
  // cursor
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorBlinking": "expand",

  // config related to code formatting
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "[javascriptreact]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "always",
    "source.fixAll.tslint": "always",
    "source.organizeImports": "always"
  },

  //terminal theme
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.fontWeight": "normal",
  "terminal.integrated.fontFamily": "JetBrains Mono",
  "workbench.colorTheme": "Andromeda Italic",
  "workbench.iconTheme": "material-icon-theme",
  "terminal.integrated.defaultProfile.windows": "Git Bash",

  // personal configure
  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.updateImportsOnFileMove.enabled": "always",
  "editor.suggestSelection": "first",
  "editor.minimap.size": "fill",
  "editor.minimap.showSlider": "always",
  "eslint.format.enable": true,
  "eslint.run": "onSave",
  "git.enableSmartCommit": true,
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "workbench.editorAssociations": {
    "*.md": "vscode.markdown.preview.editor"
  },

  "tailwindCSS.emmetCompletions": true,
  "cSpell.words": ["tailwindcss", "Asif", "iconify", "nextui"]
}
