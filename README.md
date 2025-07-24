# Visualfiles Scripting for VS Code

A Visual Studio Code extension that provides syntax highlighting and language support for Visualfiles Scripting language.

## Features

- **Syntax Highlighting**: Full syntax highlighting for Visualfiles scripting commands, variables, comments, and operators
- **Language Support**: Proper language configuration with auto-closing brackets and comment support
- **File Association**: Automatically recognizes `.vfs` and `.txt` files containing Visualfiles scripts

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

1. Open any Visualfiles script file (`.vfs` or `.txt`)
2. The syntax highlighting will automatically activate
3. Use VS Code's built-in features like:
   - Folding code blocks
   - Auto-closing brackets
   - Comment toggling (Ctrl+/)

## File Extensions

The extension recognizes these file patterns:
- `.vfs` - Dedicated Visualfiles script files
- `.txt` - Text files (commonly used for Visualfiles scripts)

## Language Features

- **Comment Support**: Use `Ctrl+/` to toggle line comments
- **Bracket Matching**: Automatic bracket pair highlighting
- **Auto-closing**: Brackets and quotes auto-close
- **Word Selection**: Double-click to select Visualfiles variables and commands
