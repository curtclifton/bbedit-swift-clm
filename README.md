# A BBEdit Codeless Language Module for Swift

## Status

Keyword, comment, and string highlighting work. Top-level classes, structs, enums, functions, and extensions are indexed and can be folded. Because of limitations in the matching power of codeless language modules, nested declarations are not indexed and are not fold-able.

## Installation

1. Copy the file *swift.plist* to *~/Library/Application Support/BBEdit/Language Modules*. You may have to create the *Langauge Modules* folder if it doesn’t exist.
2. Quit and relaunch BBEdit.

Now files with the extension “swift” should be syntax highlighted. The function popup menu in the navigation bar should also list all the declarations in the current file.

## Known Issues

- Extensions are only indexed by base type. This means that multiple extensions of the same base type have the same identifier in the function popup menu.
- Identifier matching does not include the full unicode ranges allowed by the Swift language reference. Only upper and lower case A-Z, 0-9, and ‘_’ are matched. I’m sorry for the lack of diacritic and emoji support, but I haven’t yet sorted out how to convince BBEdit to handle them in *Identifier and Keyword Character Class*.
- Because of limitations in the matching power of codeless language modules, nested declarations are not indexed and are not fold-able.

