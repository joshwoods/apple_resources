

- AppKit
- NSAlert
-  suppressionButton 

Instance Property

# suppressionButton

The alert’s suppression checkbox.

macOS 10.5+

``` source
@MainActor
var suppressionButton: NSButton? { get }
```

## Discussion

If you want to customize an alert’s suppression checkbox, access it via this property and then use the methods of the NSButton class. For example, you can do this to change the suppression checkbox’s default message, or to change its initial selection state (which is “unselected” by default). For a code example, see the showsSuppressionButton property.

## See Also

### Displaying Alerts

func runModal() -> NSApplication.ModalResponse

Runs the alert as an app-modal dialog and returns the constant that identifies the button clicked.

func beginSheetModal(for: NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Runs the alert modally as a sheet attached to the specified window.

func beginSheetModal(for: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the alert modally as an alert sheet attached to a specified window.

Deprecated

var showsSuppressionButton: Bool

Specifies whether the alert includes a suppression checkbox, which you can employ to allow a user to opt out of seeing the alert again.

