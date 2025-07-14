

- UIKit
-  UIUserNotificationSettings Deprecated

Class

# UIUserNotificationSettings

The types of notifications that can be displayed to the user by your app.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UIUserNotificationSettings
```

Deprecated

Use UNNotificationSettings instead.

## Overview

Apps that use visible or audible alerts in conjunction with a local or push notification must register the types of alerts they employ. UIKit correlates the information you provide with the user’s preferences to determine what types of alerts your app is allowed to employ.

Use this class to encapsulate your initial registration request and to view the request results. After creating an instance of this class and specifying your preferred settings, call the registerUserNotificationSettings(_:) method of the UIApplication class to register those settings. After checking your request against the user preferences, the app delivers the results to the application(_:didRegister:) method of its app delegate. The object passed to that method specifies the types of notifications that your app is allowed to use.

In addition to registering your app’s alert types, you can also use this class to register groups of custom actions to display in conjunction with local or push notifications. Custom actions represent immediate tasks your app can perform in response to the notification. You define groups of actions and associate the entire group with a given notification. When the corresponding alert is displayed, the system adds buttons for each action you specified. When the user taps the button for one of the actions, the system wakes your app and calls the application(_:handleActionWithIdentifier:forRemoteNotification:completionHandler:) or application(_:handleActionWithIdentifier:for:completionHandler:) method of its app delegate. Use those methods to perform the requested action.

## Topics

### Creating a settings object

convenience init(types: UIUserNotificationType, categories: Set&lt;UIUserNotificationCategory>?)

Creates and returns a settings object that you can use to register your requested notification and action types.

### Getting the configured settings

var types: UIUserNotificationType

A bitmask of the notification types that your app is allowed to use.

var categories: Set&lt;UIUserNotificationCategory>?

The app’s registered groups of actions.

### Constants

struct UIUserNotificationType

Constants indicating how the app alerts the user when a local or push notification arrives.

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

