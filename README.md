# VisualFiles Scripting for VS Code

A Visual Studio Code extension that provides syntax highlighting and language support for VisualFiles Scripting language.

## Features

- **Syntax Highlighting**: Full syntax highlighting for VisualFiles scripting commands, variables, comments, and operators
- **Language Support**: Proper language configuration with auto-closing brackets and comment support
- **File Association**: Automatically recognizes `.vfs` and `.txt` files containing VisualFiles scripts

## Syntax Highlighting Features

### Commands
- Control flow: `[&If]`, `[&Else]`, `[&EndIf]`, `[&DoWhile]`, `[&EndDoWhile]`
- Function calls: `[&Call]`, `[&Assign]`, `[&Show]`, `[&Message]`
- Data operations: `[&SelectRelation]`, `[&With]`, `[&EndWith]`
- System operations: `[&OSCommand]`, `[&Quit]`, `[&Out]`

### Comments
- Header blocks with asterisks (`***`)
- Line comments (`//`, `##`, `**`)
- Amendment sections

### Operators
- Assignment: `=`
- Comparison: `<=`, `>=`, `<`, `>`, `&Begins`, `&Or`
- Arithmetic: `+`, `-`, `*`, `/`
- Methods: `:l-remove`, `:proval`, `:replace`, `:choose`

## Installation

### From Source

1. Clone or download this repository
2. Copy the extension folder to your VS Code extensions directory:
   - **Windows**: `%USERPROFILE%\.vscode\extensions\`
   - **macOS**: `~/.vscode/extensions/`
   - **Linux**: `~/.vscode/extensions/`
3. Restart VS Code
4. The extension will automatically activate for `.vfs` and `.txt` files

### Manual Installation

1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Click on the `...` menu and select "Install from VSIX..."
4. Select the `.vsix` package file
5. Restart VS Code

## Usage

1. Open any VisualFiles script file (`.vfs` or `.txt`)
2. The syntax highlighting will automatically activate
3. Use VS Code's built-in features like:
   - Folding code blocks
   - Auto-closing brackets
   - Comment toggling (Ctrl+/)

## File Extensions

The extension recognizes these file patterns:
- `.vfs` - Dedicated VisualFiles script files
- `.txt` - Text files (commonly used for VisualFiles scripts)

## Language Features

- **Comment Support**: Use `Ctrl+/` to toggle line comments
- **Bracket Matching**: Automatic bracket pair highlighting
- **Auto-closing**: Brackets and quotes auto-close
- **Word Selection**: Double-click to select VisualFiles variables and commands

## Development

### Local Development

1. Clone the repository
2. Open in VS Code
3. Make your changes to the syntax files
4. Test with the included `test-sample.vfs` file
5. Run the CI validation locally: `npm install -g @vscode/vsce && vsce package`

### Continuous Integration

The project includes GitHub Actions workflows:

- **CI Workflow** (`.github/workflows/ci.yml`): Validates the extension on every push/PR
- **Publish Workflow** (`.github/workflows/publish.yml`): Automatically publishes to VS Code Marketplace on version tags

### Publishing

See [PUBLISHING.md](PUBLISHING.md) for detailed instructions on setting up automated publishing to the VS Code Marketplace.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test with sample VisualFiles scripts
5. Ensure CI passes
6. Submit a pull request

## License

MIT License - see LICENSE file for details

## Changelog

### 1.0.0
- Initial release
- Full syntax highlighting for VisualFiles scripting language
- Support for all major language constructs
- File association for .vfs and .txt files
