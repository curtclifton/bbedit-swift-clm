# A BBEdit Codeless Language Module for Swift

## Status

This is a first draft. Keyword highlighting is all that works at the moment.

## Installation

1. Copy the file *swift.plist* to *~/Application Support/BBEdit/Language Modules*. You may have to create the *Langauge Modules* folder if it doesn’t exist.
2. Quit and relaunch BBEdit.

Now files with the extension “swift” should be syntax highlighted. <!-- The function popup menu in the navigation bar should also list all the declarations in the current file. -->

## Known Issues

- No comment highlighting or even detection, so keywords in comments are incorrectly highlighted
- No function indexing
