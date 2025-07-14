

- UIKit
-  UIUserNotificationCategory Deprecated

Class

# UIUserNotificationCategory

Information about custom actions that your app can perform in response to a local or push notification.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UIUserNotificationCategory
```

Deprecated

Use UNNotificationCategory instead.

## Overview

Each instance of `UIUserNotificationCategory` represents a group of actions to display in conjunction with a single notification. The title of each action is uses as the title of a button in the alert displayed to the user. When the user taps a button, the system reports the selected action to your app delegate.

Typically, you create an instance of the UIMutableUserNotificationCategory class instead of this class. You use the mutable object to add actions and specify a category name before registering them with a UIUserNotificationSettings object.

To display a group of actions for a specific notification, configure the local or push notification with the category name of the group. For local notifications, you specify this name when configuring your UILocalNotification object. For push notifications, your server specifies a group of actions by adding a `category` key (whose value is the identifier of the group) to the push notification’s payload.

## Topics

### Creating the action group

init()

Creates an action group.

init?(coder: NSCoder)

Creates an action group from data in an unarchiver.

### Getting the group configuration

var identifier: String?

The name of the action group.

func actions(for: UIUserNotificationActionContext) -> [UIUserNotificationAction]?

Returns the actions to be displayed for the given notification context.

### Constants

enum UIUserNotificationActionContext

Constants indicating the amount of space available for displaying actions in a notification.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIMutableUserNotificationCategory

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
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

class UIUserNotificationSettings

The types of notifications that can be displayed to the user by your app.

Deprecated

