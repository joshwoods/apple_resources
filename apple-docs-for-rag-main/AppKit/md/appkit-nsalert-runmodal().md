

- AppKit
- NSAlert
-  runModal() 

Instance Method

# runModal()

Runs the alert as an app-modal dialog and returns the constant that identifies the button clicked.

macOS

``` source
@MainActor
func runModal() -> NSApplication.ModalResponse
```

## Return Value

A response to the alert. See this method’s “Special Considerations” section for details.

## Discussion

You can create the alert either through the standard allocation and initialization procedure or, if necessary in your app, by using the deprecated compatibility method alertWithMessageText:defaultButton:alternateButton:otherButton:informativeTextWithFormat:.

### Special Considerations

This method can return values other than those specific to the alert buttons (alertFirstButtonReturn, alertSecondButtonReturn, and so on) if the alert is canceled programatically.

If you use `alertWithMessageText:defaultButton:alternateButton:otherButton:informativeTextWithFormat:` to create an alert, the `NSAlertDefaultReturn`, `NSAlertAlternateReturn`, and `NSAlertOtherReturn` constants identify the button used to dismiss the alert. Otherwise, the constants used are the ones described in addButton(withTitle:).

## See Also

### Displaying Alerts

func beginSheetModal(for: NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Runs the alert modally as a sheet attached to the specified window.

func beginSheetModal(for: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the alert modally as an alert sheet attached to a specified window.

Deprecated

var suppressionButton: NSButton?

The alert’s suppression checkbox.

var showsSuppressionButton: Bool

Specifies whether the alert includes a suppression checkbox, which you can employ to allow a user to opt out of seeing the alert again.

