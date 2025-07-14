

- UIKit
-  UIMenuItem Deprecated

Class

# UIMenuItem

A custom item in the editing menu managed by the menu controller.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class UIMenuItem
```

Deprecated

Use UIEditMenuInteraction instead.

## Overview

Custom menu items appear in the menu after any validated system items. A UIMenuItem object has two properties: a title and an action selector identifying the method to invoke in the handling responder object. Targets aren’t specified; a suitable target is found via normal traversal of the responder chain. To have custom menu items appear in the editing menu, you must add them to the menuItems property of the UIMenuController object.

## Topics

### Creating a menu item

init(title: String, action: Selector)

Creates and returns a menu-item object initialized with the given title and action.

### Accessing menu-item attributes

var title: String

The title of the menu item.

var action: Selector

A selector identifying the method of the responder object to invoke for handling of the menu command.

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

### Deprecated classes

class UIActionSheet

A view that presents a set of alternatives for how to proceed with a task.

Deprecated

class UIAlertView

A view that displays an alert message.

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

