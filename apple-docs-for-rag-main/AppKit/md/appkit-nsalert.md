

- AppKit
-  NSAlert 

Class

# NSAlert

A modal dialog or sheet attached to a document window.

macOS

``` source
@MainActor
class NSAlert
```

## Overview

The methods of the NSAlert class allow you to specify alert level, alert text, button titles, and a custom icon should you require it. The class also lets your alerts display a help button and provides ways for apps to offer help specific to an alert.

To display an alert as a sheet, call the beginSheetModal(for:completionHandler:) method; to display one as an app-modal dialog, use the runModal() method.

By design, an NSAlert object is intended for a single alert—that is, an alert with a unique combination of title, buttons, and so on—that is displayed upon a particular condition. You should create an NSAlert object for each alert dialog, creating it only when you need to display an alert, and release it when you are done. If you have a particular alert dialog that you need to show repeatedly, you can retain and reuse an instance of NSAlert for this dialog.

After creating an alert using one of the alert creation methods, you can customize it further prior to displaying it by customizing its attributes. See Instance Attributes.

Unless you must maintain compatibility with existing alert-processing code that uses the function-based API, you should allocate (`alloc`) and initialize (`init`) the alert object, and then set its attributes using the appropriate methods of the `NSAlert` class.

### Instance Attributes

NSAlert objects have the following attributes:

- Type An alert’s type helps convey the importance or gravity of its message to the user. Specified with the alertStyle property.

- Message text The main message of the alert. Specified with messageText.

- Informative text Additional information about the alert. Specified with informativeText.

- Icon An optional, custom icon to display in the alert, which is used instead of the default app icon. Specified with icon.

- Help Alerts can let the user get help about them. Use helpAnchor and showsHelp.

- Response buttons By default an alert has one response button: the OK button. You can add more response buttons using the addButton(withTitle:) method.

- Suppression checkbox A suppression checkbox allows the user to suppress the display of a particular alert in subsequent occurrences of the event that triggers it. Use showsSuppressionButton.

- Accessory view An accessory view lets you add additional information to an alert; for example, a text field with contact information. Use accessoryView, layout().

### Subclassing Notes

The `NSAlert` class is not designed for subclassing.

## Topics

### Creating Alerts

init(error: any Error)

Returns an alert initialized from information in an error object.

### Configuring Alerts

func layout()

Specifies that the alert must do immediate layout instead of lazily just before display.

var alertStyle: NSAlert.Style

Indicates the alert’s severity level.

var accessoryView: NSView?

The alert’s accessory view.

var showsHelp: Bool

Specifies whether the alert has a help button.

var helpAnchor: NSHelpManager.AnchorName?

The alert’s HTML help anchor.

var delegate: (any NSAlertDelegate)?

The alert’s delegate.

### Displaying Alerts

func runModal() -> NSApplication.ModalResponse

Runs the alert as an app-modal dialog and returns the constant that identifies the button clicked.

func beginSheetModal(for: NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Runs the alert modally as a sheet attached to the specified window.

func beginSheetModal(for: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the alert modally as an alert sheet attached to a specified window.

Deprecated

var suppressionButton: NSButton?

The alert’s suppression checkbox.

var showsSuppressionButton: Bool

Specifies whether the alert includes a suppression checkbox, which you can employ to allow a user to opt out of seeing the alert again.

### Accessing Alert Text

var informativeText: String

The alert’s informative text.

var messageText: String

The alert’s message text or title.

### Accessing a Custom Alert Icon

var icon: NSImage!

The custom icon displayed in the alert.

### Accessing Alert Response Buttons

var buttons: [NSButton]

The array of response buttons for the alert.

func addButton(withTitle: String) -> NSButton

Adds a button with a given title to the alert.

### Getting Alert Windows

var window: NSWindow

The app-modal panel or document-modal sheet that corresponds to the alert.

### Constants

enum Style

The set of alert styles to style alerts in your app.

struct ModalResponse

A set of button return values for modal dialogs.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Related Documentation

Sheet Programming Topics

Dialogs and Special Panels

### Alerts

protocol NSAlertDelegate

A set of optional methods implemented by the delegate of an NSAlert object to respond to a user’s request for help.

