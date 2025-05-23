# Pancake Syntax Highlighting Extension

This VS Code extension provides syntax highlighting for the Pancake programming language.

## Features

- Syntax highlighting for Pancake language keywords, functions, variables, and more.
- Support for both light and dark color themes.

![Light Theme](asset/light.png)

*Pancake syntax highlighting with a light color theme*

![Dark Theme](asset/dark.png)

*Pancake syntax highlighting with a dark color theme*

## Installation

### Method 1: VS Code Marketplace (Recommended)
1. Open VS Code extension side tab (`Ctrl+Shift+X` (Windows, Linux) /`Cmd+Shift+X` (macOS))
2. Search for "Pancake Syntax" in the Extensions view search bar.
3. Click the "Install" button for the "Pancake Syntax" extension.
4. Once installed, the extension will be work for `.pnk` or `.🥞` files.
This way allows you to easily update the extension with changes we make.

### Method 2: Install from VSIX File
1. Download the `pancake-syntax-<version>.vsix> file from this repository
2. Open VS Code extension side tab (`Ctrl+Shift+X` (Windows, Linux) /`Cmd+Shift+X` (macOS))
3. Click the "..." menu from the right upper corner and select "Install from VSIX..."
4. Select the downloaded `.vsix` file.

**To create your own VSIX file**
1. Clone this repository: `git clone https://github.com/JunmingZhao42/pancake-vscode-highlight.git`
2. Install dependencies: `npm install`
3. Package the extension: `vsce package`

**(Optional)** For supporting better annotation highlighting, add this to your `settings.json` and adjust as needed:
```json
{
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      { "scope": "meta.specification.block.pancake",
        "settings": {
          "fontStyle": "italic"
        }},
      { "scope": "keyword.annotation.pancake",
        "settings": {
          "foreground": "#9f4575",
          "fontStyle": "bold"
        }}
    ]
  }
}
```

## Contributing

If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/JunmingZhao42/pancake-vscode-highlight.git).

---

**Enjoy coding in Pancake with enhanced syntax highlighting!**