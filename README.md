# OpenFrame Development COBOL

## Overview

OpenFrame Development COBOL for Visual Studio Code is an extension that provides COBOL editor features.

## Features

- COBOL dialect (IBM/Fujitsu)
- COBOL file format (Fixed/Variable)
- COBOL report writer, ESQL support
- Code navigation
- Highlighting
- IntelliSense
- Go to definition
- Go to references
- Hover
- Outline view
- Lint

## Commands

- `COBOL: New COBOL File` : Create a new COBOL file.
- `COBOL: Open OpenFrame Development Output panel` : Open the `OpenFrame Development` output panel.
- `COBOL: Clear metadata cache in workspace` : Clear metadata cache in workspace.
- `COBOL: Remove After column 72` : Remove all characters after column 72. (Fixed format only)
- `COBOL: Remove All Comments` : Delete all comments in the COBOL source code.
- `COBOL: Remove Sequence Numbers (Columns 1-6)` : Remove sequence numbers in columns 1-6.
- `COBOL: Renumber Sequence Numbers (Columns 1-6)` : Renumber sequence numbers in columns 1-6.

## Settings

- `cobol.intellisenseCobolDialect` : Select COBOL dialect for IntelliSense. **(IBM/Fujitsu)**
- `cobol.intellisenseReportWriter` : Enable Report Writer for IntelliSense.
- `cobol.fileFormat` : Set COBOL File format. **(fixed/variable)**
- `cobol.copybookDirectory` : Set the directories to search for COBOL Copybooks.
- `cobol.lint` : Enable linting for COBOL code.
- `cobol.lintUnusedSections` : Enable linting for unused sections.
- `cobol.lintUnusedParagraphs` : Enable linting for unused paragraphs.
- `cobol.lintUnusedVariables` : Enable linting for unused variables.
- `cobol.referenceCodeLens` : Enable CodeLens to show references.

## Shortcuts

| Keys              | Description |
| ----------------- | ------------------------------------------- |
| `Ctrl+Alt+R`      | Move to the **PROCEDURE DIVISION**. |
| `Ctrl+Alt+W`      | Move to the **WORKING-STORAGE SECTION**. |
| `Ctrl+Alt+D`      | Move to the **DATA DIVISION**. |
| `Ctrl+Alt+Q`      | Move **backward** to the previous division or section. |
| `Ctrl+Alt+E`      | Move **forward** to the next division or section. |
| `Alt+RightArrow`  | Insert spaces up to **column 72**. |
| `Ctrl+/`          | Toggle COBOL comment/uncomment for selected lines of code. |
| `Ctrl+Alt+;`      | Decrease indentation level for selected lines of code. |
| `Ctrl+Alt+'`      | Increase indentation level for selected lines of code. |

## Menus

- Align Storage Keyword : Aligns storage declarations according to the chosen alignment option. (First Line, Leftmost, Center, Rightmost)
- Convert Selection : Converts the selected text between hexadecimal and ASCII formats.

## Requirements

- VS Code (version 1.85.2 or later)

## Examples

### IntelliSense

#### Full source

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/intellisense1.gif)

#### Code snippet

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/intellisense2.gif)

### Go to Definition, References

#### Variable/section/paragraph

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/goto_find_reference.gif)

#### CopyBook

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/goto_definition2.gif)

### Hover

#### Data

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/hover1.gif)

#### Hex value

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/hover2.png)

#### Language Environment callable service

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/hover3.png)

### Outline

#### Outline view explorer

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/outline1.gif)

#### Outline view search

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/outline2.gif)

### Commands, Menus

#### Comment/uncomment, indent/outdent

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/command.gif)

#### Move to PROCEDURE/DATA DIVISION, WORKING-STORAGE SECTION, Next/Previous

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/move.gif)

#### Align Storage Keyword

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/data_align.gif)

### Lint

![](https://raw.githubusercontent.com/Tmaxsoft-Compiler/vscode-ofstudio/refs/heads/main/doc/lint.png)

## License

This extension utilizes the following open source components and is distributed under the licenses described below:

- vscode_cobol (25.1.1)
  - License: MIT License
  - Copyright
    - (c) 2015-2020 Stephen Gennard
    - (c) 2021-2025 Stephen Paul Gennard
  - [License](https://github.com/spgennard/vscode_cobol/blob/main/LICENSE)
