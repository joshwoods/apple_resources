

- AppKit
- NSSavePanel
-  begin(completionHandler:) 

Instance Method

# begin(completionHandler:)

Presents the panel as a modeless window.

macOS 10.6+

``` source
@MainActor
func begin(completionHandler handler: @escaping (NSApplication.ModalResponse) -> Void)
```

``` source
@MainActor
func begin() async -> NSApplication.ModalResponse
```

## Parameters 

`handler`  

The block to call after the user closes the panel. This block has no return value and takes a single parameter:

result  
The action taken by the user. The value of this parameter is NSFileHandlingPanelOKButton if the user chose the OK button or NSFileHandlingPanelCancelButton if the user chose the Cancel button.

## Discussion

Configure all of the relevant properties of the panel before you call this method.

## See Also

### Showing the Panel

func beginSheetModal(for: NSWindow, completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a sheet modal to the specified window.

func runModal() -> NSApplication.ModalResponse

Displays the panel and begins its event loop with the current working (or last-selected) directory as the default starting point.

func validateVisibleColumns()

Validates and reloads the browser columns visible in the panel.

