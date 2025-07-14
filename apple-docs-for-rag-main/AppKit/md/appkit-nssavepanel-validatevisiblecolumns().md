

- AppKit
- NSSavePanel
-  validateVisibleColumns() 

Instance Method

# validateVisibleColumns()

Validates and reloads the browser columns visible in the panel.

macOS

``` source
@MainActor
func validateVisibleColumns()
```

## Discussion

Call this method to validate the contents of the panel. For example, you might call it to allow the selection of files with certain extensions based on the selection made in an accessory-view pop-up list. When the user changes the selection, invoke this method to revalidate the visible columns.

## See Also

### Showing the Panel

func beginSheetModal(for: NSWindow, completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a sheet modal to the specified window.

func begin(completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a modeless window.

func runModal() -> NSApplication.ModalResponse

Displays the panel and begins its event loop with the current working (or last-selected) directory as the default starting point.

