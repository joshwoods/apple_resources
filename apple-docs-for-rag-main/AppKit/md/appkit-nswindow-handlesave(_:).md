

- AppKit
- NSWindow
-  handleSave(\_:) 

Instance Method

# handleSave(\_:)

Handles the AppleScript command to save the window (and its associated document, if any).

macOS

``` source
@MainActor
func handleSave(_ command: NSScriptCommand) -> Any?
```

## Discussion

If there’s a corresponding document and the window is the main window of the document, it forwards the `save` command to the corresponding document. Otherwise, this method does nothing.

## See Also

### Handling Script Commands

func handleClose(NSCloseCommand) -> Any?

Handles the AppleScript command to close the window (and its associated document, if any).

func handlePrint(NSScriptCommand) -> Any?

Handles the AppleScript command to print the contents of the window (or its associated document, if any).

