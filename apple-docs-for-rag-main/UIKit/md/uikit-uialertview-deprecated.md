

- UIKit
-  UIAlertView Deprecated

Class

# UIAlertView

A view that displays an alert message.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UIAlertView
```

Deprecated

Instead, use UIAlertController with a preferredStyle of UIAlertController.Style.alert.

## Overview

In apps that run in versions of iOS prior to iOS 8, use the UIAlertView class to display an alert message to the user. An alert view functions similar to but differs in appearance from an action sheet (an instance of UIActionSheet).

### Using an alert view

Use the properties and methods defined in this class to set the title, message, and delegate of an alert view and configure the buttons in apps that run in versions of iOS prior to iOS 8. You must set a delegate if you add custom buttons. The delegate should conform to the UIAlertViewDelegate protocol. Use the show() method to display an alert view after it’s configured.

### Subclassing notes

The UIAlertView class is intended to be used as-is and doesn’t support subclassing. The view hierarchy for this class is private and must not be modified.

## Topics

### Creating alert views

convenience init(title: String?, message: String?, delegate: Any?, cancelButtonTitle: String?)

Convenience method for initializing an alert view.

convenience init(title: String, message: String, delegate: (any UIAlertViewDelegate)?, cancelButtonTitle: String?, otherButtonTitles: String, String...)

Creates an alert view with the specified values.

init(frame: CGRect)

Creates an alert view with the specified frame.

init?(coder: NSCoder)

Creates an alert view from data in an unarchiver.

### Setting properties

var delegate: AnyObject?

The receiver’s delegate or `nil` if it doesn’t have a delegate.

var alertViewStyle: UIAlertViewStyle

The kind of alert displayed to the user.

var title: String

The string that appears in the receiver’s title bar.

var message: String?

Descriptive text that provides more details than the title.

var isVisible: Bool

A Boolean value that indicates whether the receiver is displayed.

### Configuring buttons

func addButton(withTitle: String?) -> Int

Adds a button to the receiver with the given title.

var numberOfButtons: Int

The number of buttons on the alert view.

func buttonTitle(at: Int) -> String?

Returns the title of the button at the given index.

func textField(at: Int) -> UITextField?

Returns the text field at the given index

var cancelButtonIndex: Int

The index number of the cancel button.

var firstOtherButtonIndex: Int

The index of the first other button.

### Displaying

func show()

Displays the receiver using animation.

### Dismissing

func dismiss(withClickedButtonIndex: Int, animated: Bool)

Dismisses the receiver, optionally with animation.

### Constants

enum UIAlertViewStyle

The presentation style of the alert.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Deprecated classes

class UIActionSheet

A view that presents a set of alternatives for how to proceed with a task.

Deprecated

class UIDocumentMenuViewController

A list of all the available document providers for a given file type and mode, in addition to custom menu items that you add.

Deprecated

class UILocalNotification

A notification that an app can schedule for presentation at a specific date and time.

Deprecated

class UIMenuController

The menu interface for the Cut, Copy, Paste, Select, Select All, and Delete commands.

Deprecated

class UIMenuItem

A custom item in the editing menu managed by the menu controller.

Deprecated

class UIMutableUserNotificationAction

A modifiable version of the user notification action class.

Deprecated

class UIMutableUserNotificationCategory

Information about custom actions that your app can perform in response to a local or push notification.

Deprecated

class UIPopoverController

An object that manages the presentation of content in a popover.

Deprecated

class UIPreviewAction

A preview action, or *peek quick action*, that displays below a peek when a user swipes the peek upward.

Deprecated

class UIPreviewActionGroup

A group of one or more child quick actions, each an instance of the preview action class.

Deprecated

class UISearchDisplayController

An object that manages the display of a search bar, along with a table view that displays search results.

Deprecated

class UIStoryboardPopoverSegue

A specific type of segue for presenting content in a popover.

Deprecated

class UIUserNotificationAction

A custom action that your app can perform in response to a remote or local notification.

Deprecated

class UIUserNotificationCategory

Information about custom actions that your app can perform in response to a local or push notification.

Deprecated

class UIUserNotificationSettings

The types of notifications that can be displayed to the user by your app.

Deprecated

