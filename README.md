# VSCode Settings Repository

This repository contains the configuration file for my Visual Studio Code (VSCode) settings, stored in the `settings.json` file. These settings include customizations for editor behavior, terminal profiles, C++ development, Vim keybindings, and various extensions. It is structured to optimize workflow and productivity.

## Settings Overview

### General Editor Settings
- **Cursor Smooth Caret Animation**: Enabled for smoother visual feedback while typing (`"editor.cursorSmoothCaretAnimation": "on"`).
- **Smooth Scrolling**: Enabled for editor, terminal, and explorer (`"editor.smoothScrolling": true`).
- **Tab Size**: Set to 2 spaces for consistent indentation (`"editor.tabSize": 2`).
- **Confirmation Dialog**: Disabled for delete actions in the explorer (`"explorer.confirmDelete": false`).

### Terminal Profiles
Custom terminal profiles are defined for PowerShell, Command Prompt, Git Bash, and MSYS2 Bash:
- **Windows PowerShell**: Default profile (`"terminal.integrated.defaultProfile.windows": "Windows PowerShell"`).
- **Git Bash**: Source for Git Bash (`"terminal.integrated.profiles.windows"`).

### C++ Development
VSCode is configured to work with C++ using `gcc` and `clangFormat`:
- **Compiler Path**: Set to `C:\msys64\ucrt64\bin\g++.exe` (`"C_Cpp.default.compilerPath"`).
- **Formatting**: Uses `clangFormat` with Google style for C++ (`"C_Cpp.clang_format_fallbackStyle": "{ BasedOnStyle: Google, IndentWidth: 2, ColumnLimit: 0}"`).
- **Formatter**: Set to `ms-vscode.cpptools` for C++ files.

### Vim Keybindings
Enhanced Vim keybindings are set up for navigation, editing, and command execution:
- **Insert Mode**: Quick exit from insert mode using `jk`
- **Normal Mode**: Custom keybindings for common actions:
  - `Space + w`: Save file.
  - `Space + o`: Focus sidebar.
  - `Space + e`: Toggle sidebar.
  - `Space + c`: Close active tab.
  - `g d`: Go to definition.
  - `Space + /`: Toggle comments.
  - `Space + l r`: Rename variables.
  - `Space + d b`: Toggle breakpoints.
  - `Space + d c`: Start debugging.

- **Visual Mode**: Indentation and comment toggle with custom keybindings.

### Appearance
- **Font**: Set to 18pt with a font weight of 300 for optimal readability (`"editor.fontSize": 18`, `"editor.fontWeight": "300"`).
- **Line Numbers**: Relative line numbers are enabled for easier navigation (`"editor.lineNumbers": "relative"`).
- **Theme**: The Catppuccin Mocha theme is used for a visually pleasing interface (`"workbench.colorTheme": "Catppuccin Mocha"`).
- **Zoom Level**: Slightly zoomed out for better workspace view (`"window.zoomLevel": -1`).

### Indentation Rainbow
- The Indentation Rainbow extension is configured to show progressively lighter colors for each indentation level to improve code structure visualization.

### Miscellaneous
- **Makefile and CMake**: Makefile and CMake settings are specified for project automation.
- **Workspace Trust**: The workspace is configured to automatically open untrusted files without confirmation (`"security.workspace.trust.untrustedFiles": "open"`).
