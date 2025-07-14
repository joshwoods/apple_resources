

- AppKit
- NSWindow
-  handlePrint(\_:) 

Instance Method

# handlePrint(\_:)

Handles the AppleScript command to print the contents of the window (or its associated document, if any).

macOS

``` source
@MainActor
func handlePrint(_ command: NSScriptCommand) -> Any?
```

## Discussion

If there’s a corresponding document and the window is the main window of the document, it forwards the `print` command to the corresponding document. Otherwise, the window sends itself a `print` message.

## See Also

### Handling Script Commands

func handleClose(NSCloseCommand) -> Any?

Handles the AppleScript command to close the window (and its associated document, if any).

func handleSave(NSScriptCommand) -> Any?

Handles the AppleScript command to save the window (and its associated document, if any).

