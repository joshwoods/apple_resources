

- UIKit
-  UIMutableUserNotificationAction Deprecated

Class

# UIMutableUserNotificationAction

A modifiable version of the user notification action class.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UIMutableUserNotificationAction
```

Deprecated

Use UNNotificationAction instead.

## Overview

When a notification is delivered, the system displays a button for each custom action associated with the notification. Tapping a button launches your app (either in the foreground or background) and gives you a chance to perform the indicated action. You use this class to configure the details about the button that is displayed and the information your app needs to perform the corresponding action.

To associate custom actions with a local or remote notification, create one or more instances of this class and use them to configure one or more UIMutableUserNotificationActionSettings objects. An action settings objects defines the set of actions to associate with a single notification. You register your app’s action settings objects at launch time, along with your app’s preferred notification options, using a UIUserNotificationSettings object.

For each action you define, you must specify whether execution of that action requires the app to be running in the foreground or background. You can also specify whether the device must be unlocked or can remain locked while the action is performed. Unlocking the device may be necessary if the action involves reading or writing files that are encrypted on disk using the system’s data protection mechanism. When the user selects an action, the system puts your app into the appropriate mode and calls your app delegate’s application(_:handleActionWithIdentifier:forRemoteNotification:completionHandler:) or application(_:handleActionWithIdentifier:for:completionHandler:) method to perform the action.

## Topics

### Getting the action information

var identifier: String?

The string that you use internally to identify the action.

var title: String?

The localized string to use as the button title for the action.

### Configuring the action’s behavior

var activationMode: UIUserNotificationActivationMode

The mode in which to run the app when the action is performed.

var isAuthenticationRequired: Bool

A Boolean value indicating whether the user must unlock the device before the action is performed.

var isDestructive: Bool

A Boolean value indicating whether the action is destructive.

var behavior: UIUserNotificationActionBehavior

The custom behavior (if any) that the action supports.

var parameters: [AnyHashable : Any]

A dictionary of additional parameters to include with the action.

## Relationships

### Inherits From

- UIUserNotificationAction

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

