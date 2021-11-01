# Visual Studio Keymap for Visual Studio Code

This extension ports popular Visual Studio keyboard shortcuts to Visual Studio Code. After installing the extension and restarting VS Code your favorite keyboard shortcuts from Visual Studio are now available. 

## What keyboard shortcuts are included?

| Command | Key | 
| ----------- | ----------- |
| `workbench.action.tasks.build` | `ctrl+shift+b` |
| `editor.action.selectHighlights` | `shift+alt+oem_1` |
| `workbench.debug.viewlet.action.addFunctionBreakpointAction` | `ctrl+b` |
| `workbench.debug.viewlet.action.removeAllBreakpoints` | `ctrl+shift+f9` |
| `workbench.action.debug.restart` | `ctrl+shift+f5` |
| `editor.debug.action.runToCursor` | `ctrl+f10` |
| `settings.action.editFocusedSetting` | `alt+enter` |
| `settings.action.editFocusedSetting` | `ctrl+oem_period` |
| `problems.action.showQuickFixes` | `alt+enter` |
| `problems.action.showQuickFixes` | `ctrl+oem_period` |
| `editor.action.quickFix` | `alt+enter` |
| `editor.action.quickFix` | `ctrl+oem_period` |
| `editor.action.formatDocument` | `ctrl+k ctrl+d` |
| `editor.action.formatDocument.none` | `ctrl+k ctrl+d` |
| `insertSnippet` | `ctrl+k ctrl+x` |
| `editor.action.deleteLines` | `ctrl+shift+l` |
| `editor.action.clipboardCutAction` | `ctrl+l` |
| `workbench.action.files.openFileFolder` | `ctrl+shift+g` |
| `editor.action.referenceSearch.trigger` | `alt+f12` |
| `redo` | `ctrl+y` |
| `editor.action.smartSelect.expand` | `shift+alt+oem_plus` |
| `editor.action.addSelectionToNextFindMatch` | `shift+alt+oem_period` |
| `editor.action.triggerSuggest` | `ctrl+alt+space` |
| `undo` | `alt+space` |
| `deleteWordEndRight` | `ctrl+delete` |
| `deleteWordStartLeft` | `ctrl+backspace` |
| `workbench.action.files.saveAll` | `ctrl+shift+s` |
| `workbench.action.output.toggleOutput` | `ctrl+alt+o` |
| `workbench.view.explorer` | `ctrl+alt+l` |
| `editor.action.rename` | `ctrl+r ctrl+r` |
| `editor.action.toggleRenderWhitespace` | `ctrl+r ctrl+w` |
| `editor.foldAll` | `ctrl+m ctrl+o` |
| `editor.unfoldAll` | `ctrl+m ctrl+l` |
| `workbench.action.navigateBack` | `ctrl+-` |
| `workbench.action.navigateForward` | `ctrl+shift+-` |
| `workbench.action.quickOpen` | `ctrl+,` |
| `cursorColumnSelectDown` | `shift+alt+down` |
| `cursorColumnSelectLeft` | `shift+alt+left` |
| `cursorColumnSelectPageDown` | `shift+alt+pagedown` |
| `cursorColumnSelectPageUp` | `shift+alt+pageup` |
| `cursorColumnSelectRight` | `shift+alt+right` |
| `cursorColumnSelectUp` | `shift+alt+up` |
| `workbench.action.toggleZenMode` | `shift+alt+enter` |
| `workbench.action.closeActiveEditor` | `ctrl+f4` |
| `editor.action.copyLinesDownAction` | `ctrl+d` |
| `cursorWordStartRight` | `ctrl+right` |
| `cursorWordStartRightSelect` | `ctrl+shift+right` |
| `editor.action.insertLineBefore` | `ctrl+enter` |
| `editor.action.insertLineAfter` | `shift+enter` |
| `editor.action.wordHighlight.next` | `ctrl+shift+down` |
| `editor.action.wordHighlight.prev` | `ctrl+shift+up` |
| `editor.action.replaceAll` | `alt+a` |
| `search.action.replaceAll` | `alt+a` |
| `search.action.replaceAllInFile` | `alt+a` |
| `search.action.replaceAllInFolder` | `alt+a` |
| `editor.action.replaceOne` | `alt+r` |
| `search.action.replace` | `alt+r` |
| `toggleSearchRegex` | `alt+e` |
| `toggleFindRegex` | `alt+e` |
| `deleteWordStartRight` | `ctrl+delete` |
| `editor.action.toUpperCase` | `ctrl+shift+u` |
| `editor.action.toLowerCase` | `ctrl+u` |
| `editor.action.jumpToBracket` | `ctrl+oem_6` |
| `editor.action.formatSelection` | `ctrl+k ctrl+c` |

The full list of keyboard shortcuts including the `when` clause (e.g. while debugging) can be found in the extension's [contribution list](https://github.com/microsoft/vscode-vs-keybindings/blob/bf87aaa88a7e50e4c316ce3f4fe703c4443366ce/package.json#L26). 

## Why don't all the keyboard shortcuts work? 

VS Code does not implement all of the commands available in Visual Studio. If you would like to see a feature in VS Code that is in Visual Studio, please open an [issue on GitHub](https://github.com/Microsoft/vscode/issues/new). 

## How do I contribute a keyboard shortcut?

We may have missed a keyboard shortcut. If we did please help us out! It is very easy to make a PR. 

1. Head over to our [GitHub repository](https://github.com/Microsoft/vscode-vs-keybindings). 
2. Open [`package.json`](https://github.com/Microsoft/vscode-vs-keybindings/blob/main/package.json). 
3. Add a JSON object to [`contributes.keybindings`](https://github.com/Microsoft/vscode-vs-keybindings/blob/main/package.json#L26) as seen below. 
4. Open a pull request. 

```json
{
    "mac": "<keyboard shortcut for mac>",
    "linux": "<keyboard shortcut for linux>",
    "win": "<keyboard shortcut for windows>",
    "key": "<default keyboard shortcut>",
    "command": "<name of the command in VS Code>"
}
```

You can read more about how to contribute keybindings in extensions in the [official documentation](http://code.visualstudio.com/docs/extensionAPI/extension-points#_contributeskeybindings). 
