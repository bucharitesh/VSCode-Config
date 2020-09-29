# VS Code Settings
These are some minor tweaks, I use on a day to day basis. These tweaks are mostly used for my WebDev purpose. Feel free to add more tweaks :) <3

## Themes/Color

* Current theme:
  * [Just Black](https://marketplace.visualstudio.com/items?itemName=nur.just-black)
* [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
* [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=coenraads.bracket-pair-colorizer)
  * Matching parenthesis and curly brackets to with colors
  
## IntelliSense/AutoComplete

* [IntelliSense for CSS class names in HTML](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
  * Provides CSS class name completion for the HTML class attribute based on the definitions found in your workspace or external files referenced through the link element
* [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
  * Autocompletes npm modules in import/require statements
* [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
  * Autocompletes filenames
* [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur)
  * Vue tooling

## Style/Formatting

* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  * Integrates ESLint JS
* [Beautify](https://marketplace.visualstudio.com/items?itemName=hookyqr.beautify)
  * Automatically format javascript, JSON, CSS, Sass, and HTML files.

## Useful/Extra

* [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
  * Display inline the size of the required/imported package
* [Quokka.js](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode)
  * Evaluate code/logs inline and show results in the editor
* [VS Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)
  * Collaborative editing, debugging, and more inside VS Code

# Settings

```json
{
  /* Editor config */
  "editor.lineNumbers": "on",
  "editor.fontFamily": "Fira Code, Consolas, 'Courier New', monospace",
  "editor.fontLigatures": true,
  "editor.fontSize": 16,
  "editor.tabSize": 4,
  "editor.insertSpaces": true,
  "editor.detectIndentation": false,
  "editor.renderIndentGuides": false,
  "editor.hover.enabled": true,
  "editor.cursorStyle": "line",
  "editor.wordWrap": "on",
  "editor.overviewRulerBorder": false,
  "editor.renderLineHighlight": "none",
  "editor.fontWeight": "400",
  "editor.cursorBlinking": "solid",
  "editor.semanticHighlighting.enabled": true,
  "editor.colorDecorators": false,
  "editor.minimap.enabled": false,
  "editor.tabCompletion": "on",
  "editor.glyphMargin": false, // used for debugging
  "editor.snippetSuggestions": "top",
  "editor.parameterHints.enabled": false,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "editor.showFoldingControls": "mouseover",
  "editor.find.seedSearchStringFromSelection": true,
  "editor.renderWhitespace": "none",
  "editor.renderControlCharacters": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "editor.matchBrackets": "always",
  "editor.formatOnPaste": true,
  "editor.wordBasedSuggestions": false,
  "editor.lineHeight": 0,
  "editor.suggestSelection": "first",
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": ["comment", "comment.block"],
      },
      {
        "scope": [
          "keyword.operator.logical",
          "keyword.operator.arithmetic",
          "keyword.operator.assignment",
          "keyword.operator.bitwise"
        ],
        "settings": {
          "fontStyle": ""
        }
      }
    ]
  },

  /* VS code Config */
  "window.zoomLevel": 0,
  "workbench.iconTheme": "vscode-icons",
  "workbench.editor.tabSizing": "shrink",
  "workbench.editor.limit.enabled": true,
  "workbench.editor.limit.value": 10,
  "workbench.editor.tabCloseButton": "off",
  "workbench.editor.enablePreviewFromQuickOpen": false,
  "workbench.startupEditor": "newUntitledFile",
  "workbench.colorTheme": "Tokyo Night",
  "workbench.statusBar.visible": false,
  "window.title": "${dirty} ${rootName}",
  "files.defaultLanguage": "${activeEditorLanguage}",

  /* Terminal Config */
  "terminal.integrated.rendererType": "dom",
  "terminal.integrated.fontSize": 12,

  /* Emmet config */
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "vue-html": "html"
  },
  "emmet.showAbbreviationSuggestions": true,

  /* Live Share */
  "liveshare.featureSet": "insiders",

  // Html config
  "html.format.enable": true,
  "html.format.preserveNewLines": true,

  // Javascript config
  "javascript.validate.enable": false,
  "javascript.format.enable": false,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "javascript.suggest.names": false,

  /* Eslint */
  "eslint.validate": [
    {
      "language": "vue",
      "autoFix": true
    },
    {
      "language": "typescript",
      "autoFix": true
    },
    {
      "language": "html",
      "autoFix": true
    },
    {
      "language": "javascript",
      "autoFix": true
    }
  ],

  /* File Formatter & Beautifier */
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[json]": {
    "editor.defaultFormatter": "HookyQR.beautify"
  },

  "[html]": {
    "editor.defaultFormatter": "HookyQR.beautify"
  },

  "[css]": {
    "editor.defaultFormatter": "HookyQR.beautify"
  },

  "[vue]": {
    "editor.defaultFormatter": "octref.vetur"
  },

  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[scss]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "beautify.language": {
    "css": ["css", "scss"],
    "html": ["htm", "html", "njk", "pug", "liquid", "php", "erb"],
    "js": {
      "filename": [".jshintrc", ".jsbeautify"],
      "type": ["javascript", "json"]
    }
  },

  /* Misc Config*/
  "sync.autoDownload": true,
  "sync.quietSync": true,
  "todo-tree.tree.showScanModeButton": false,
  "diffEditor.ignoreTrimWhitespace": false,
  "liveshare.anonymousGuestApproval": "accept"
}

```
