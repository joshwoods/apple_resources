

- AppKit
- NSSavePanel
-  runModal() 

Instance Method

# runModal()

Displays the panel and begins its event loop with the current working (or last-selected) directory as the default starting point.

macOS

``` source
@MainActor
func runModal() -> NSApplication.ModalResponse
```

## Return Value

`NSFileHandlingPanelOKButton` (if the user clicks the OK button) or `NSFileHandlingPanelCancelButton` (if the user clicks the Cancel button).

## Discussion

This method invokes `NSApplication`’s runModal(for:) method with `self` as the argument.

## See Also

### Related Documentation

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

### Showing the Panel

func beginSheetModal(for: NSWindow, completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a sheet modal to the specified window.

func begin(completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a modeless window.

func validateVisibleColumns()

Validates and reloads the browser columns visible in the panel.

