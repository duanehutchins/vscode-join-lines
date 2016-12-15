# Join Lines Extension for Visual Studio Code

## As of VSCode version 1.8.0, this extention is no longer necessary

To use the built-in editor join functionality, add "editor.action.joinLines" to your keybindings.

```
{ "key": "ctrl+j", "command": "editor.action.joinLines", "when": "editorTextFocus" }
```

## Feature Overview

Use Ctrl+j | ⌘+j to join lines, just like in Atom and similar to Sublime Text: the next line is joined to
the current line, and all whitespace is replaced with a single space.

![join-lines-preview](https://cloud.githubusercontent.com/assets/2899448/11255751/36ee036a-8e48-11e5-8e1f-8889bf2df026.gif)

## Install

Launch VS Code Quick Open (Ctrl/Cmd+P), paste the following command, and press enter.
```
ext install join-lines
```

## Functionality in Detail

The Rules are:
* If nothing is selected, the current line is joined with the next, and the cursor position is moved to the end
of the original line (minus whitespace)
* If text is selected, and it's all on one line, the current line is joined with the next, and the selection is retained
* If text is selected, and it spans multiple lines, the selected lines are joined, and the selection is retained (minus whitespace)

Multiple selections are also supported.

## Support

[Create an issue](https://github.com/wmaurer/vscode-join-lines/issues), or ping [@waynemaurer](https://twitter.com/waynemaurer) on Twitter.
