

- AppKit
- NSSavePanel
-  beginSheetModal(for:completionHandler:) 

Instance Method

# beginSheetModal(for:completionHandler:)

Presents the panel as a sheet modal to the specified window.

macOS 10.6+

``` source
@MainActor
func beginSheetModal(
    for window: NSWindow,
    completionHandler handler: @escaping (NSApplication.ModalResponse) -> Void
)
```

``` source
@MainActor
func beginSheetModal(for window: NSWindow) async -> NSApplication.ModalResponse
```

## Parameters 

`window`  

The window in which the panel will be presented.

`handler`  

The block called after the user dismisses the panel. The argument passed in will be NSFileHandlingPanelOKButton if the user chose the OK button or NSFileHandlingPanelCancelButton if the user chose the Cancel button.

## Discussion

Configure all the relevant properties of the panel before you call this method. The completion handler block runs after the user dismisses the panel, but while the panel may still be onscreen. If you need to dismiss the panel from the screen—for example, if the completion block displays an alert—close the panel by calling its orderOut(_:) method with the value `nil`.

## See Also

### Showing the Panel

func begin(completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a modeless window.

func runModal() -> NSApplication.ModalResponse

Displays the panel and begins its event loop with the current working (or last-selected) directory as the default starting point.

func validateVisibleColumns()

Validates and reloads the browser columns visible in the panel.

