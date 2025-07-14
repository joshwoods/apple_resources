

- UIKit
-  UIDocumentMenuViewController Deprecated

Class

# UIDocumentMenuViewController

A list of all the available document providers for a given file type and mode, in addition to custom menu items that you add.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UIDocumentMenuViewController
```

Deprecated

Use UIDocumentPickerViewController instead.

## Topics

### Creating a document menu

init(documentTypes: [String], in: UIDocumentPickerMode)

Initializes and returns a document menu to import or open the given file types.

init(url: URL, in: UIDocumentPickerMode)

Initializes and returns a document menu to export or move the given document.

init?(coder: NSCoder)

Creates a document menu from data in an unarchiver.

### Getting the user-selected document picker

var delegate: (any UIDocumentMenuDelegate)?

The document menu’s delegate.

protocol UIDocumentMenuDelegate

A set of methods that you must implement to track user interactions with a document menu view controller.

### Configuring a document menu

func addOption(withTitle: String, image: UIImage?, order: UIDocumentMenuOrder, handler: () -> Void)

Adds a custom menu item to the list of document pickers.

enum UIDocumentMenuOrder

The insertion point for custom menu items.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Deprecated classes

class UIActionSheet

A view that presents a set of alternatives for how to proceed with a task.

Deprecated

class UIAlertView

A view that displays an alert message.

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

