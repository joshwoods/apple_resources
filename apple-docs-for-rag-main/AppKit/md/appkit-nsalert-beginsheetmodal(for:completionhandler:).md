

- AppKit
- NSAlert
-  beginSheetModal(for:completionHandler:) 

Instance Method

# beginSheetModal(for:completionHandler:)

Runs the alert modally as a sheet attached to the specified window.

macOS 10.9+

``` source
@MainActor
func beginSheetModal(
    for sheetWindow: NSWindow,
    completionHandler handler: ((NSApplication.ModalResponse) -> Void)? = nil
)
```

``` source
@MainActor
func beginSheetModal(for sheetWindow: NSWindow) async -> NSApplication.ModalResponse
```

## Parameters 

`sheetWindow`  

The window on which to display the sheet.

`handler`  

The completion handler that gets called when the sheet’s modal session ends.

## Discussion

This method uses the `NSWindow` sheet methods to display the alert (for more information, see Managing Sheets). If the alert has an alert style of NSCriticalAlertStyle, it is presented as a critical sheet, which means that it can display on top of other sheets that might already be attached to the window. Otherwise, it is presented—or queued for presentation—as a standard sheet.

Note that orderOut(_:) no longer needs to be called in the completion handler. If you don’t dismiss the alert, it will be done for you after the completion handler finishes.

## See Also

### Displaying Alerts

func runModal() -> NSApplication.ModalResponse

Runs the alert as an app-modal dialog and returns the constant that identifies the button clicked.

func beginSheetModal(for: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the alert modally as an alert sheet attached to a specified window.

Deprecated

var suppressionButton: NSButton?

The alert’s suppression checkbox.

var showsSuppressionButton: Bool

Specifies whether the alert includes a suppression checkbox, which you can employ to allow a user to opt out of seeing the alert again.

