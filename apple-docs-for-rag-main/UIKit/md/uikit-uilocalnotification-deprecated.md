

- UIKit
-  UILocalNotification Deprecated

Class

# UILocalNotification

A notification that an app can schedule for presentation at a specific date and time.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
class UILocalNotification
```

Deprecated

Use UNNotificationRequest instead.

## Overview

The operating system is responsible for delivering local notifications at their scheduled times; the app does not have to be running for this to happen. Although local notifications are similar to remote notifications in that they are used for displaying alerts, playing sounds, and badging app icons, they are composed and delivered locally and do not require connection with remote servers.

Local notifications are primarily intended for apps with timer-based behaviors and simple calendar or to-do list apps. An app that is running in the background may also schedule a local notification to inform the user of an incoming message, chat, or update. An app can have only a limited number of scheduled notifications; the system keeps the soonest-firing 64 notifications (with automatically rescheduled notifications counting as a single notification) and discards the rest.

When you create a local notification, you must specify either a specific date or a geographic region as the trigger for delivering the notification. Date-based notifications are delivered at the day and time you specify, and allowances can be made for time zone changes as needed. Region-based notifications are delivered when the user enters or exits the specified region. In both cases, you can specify whether the notifications are one-time events or can be rescheduled and delivered again.

After creating a `UILocalNotification` object, schedule it using either the scheduleLocalNotification(_:) or presentLocalNotificationNow(_:) method of the UIApplication class. The scheduleLocalNotification(_:) method uses the fire date to schedule delivery; the presentLocalNotificationNow(_:) method presents the notification immediately, regardless of the value of `fireDate`. You can cancel one or more local notifications using the cancelLocalNotification(_:) or cancelAllLocalNotifications() method of the UIApplication object.

When the system delivers a local notification, several things can happen, depending on the app state and the type of notification. If the app is not frontmost and visible, the system displays the alert message, badges the app, and plays a sound—whatever is specified in the notification. If the notification is an alert and the user taps the action button (or, if the device is locked, drags open the action slider), the app is woken up or launched. (If the user taps one of the custom actions you specify using the category property, the app is woken up or launched into the background.) In its application(_:didFinishLaunchingWithOptions:) method, the app delegate can obtain the `UILocalNotification` object from the launch options dictionary using the localNotification key. The delegate can inspect the properties of the notification and, if the notification includes custom data in its userInfo dictionary, it can access that data and process it accordingly. On the other hand, if the local notification only badges the app icon, and the user in response launches the app, the application(_:didFinishLaunchingWithOptions:) method is called, but no `UILocalNotification` object is included in the options dictionary. When the user selects a custom action, the app delegate’s application(_:handleActionWithIdentifier:for:completionHandler:) method is called to handle the action.

If the app is foremost and visible when the system delivers the notification, the app delegate’s application(_:didReceive:) is called to process the notification. Use the information in the provided `UILocalNotification` object to decide what action to take. The system does not display any alerts, badge the app’s icon, or play any sounds when the app is already frontmost.

An app is responsible for managing the badge number displayed on its icon. For example, if a text-messaging app processes all incoming messages after receiving a local notification, it should remove the icon badge by setting the applicationIconBadgeNumber property of the UIApplication object to 0.

## Topics

### Scheduling a local notification

var fireDate: Date?

The date and time when the system should deliver the notification.

var timeZone: TimeZone?

The time zone of the notification’s fire date.

var repeatInterval: NSCalendar.Unit

The calendar interval at which to reschedule the notification.

var repeatCalendar: Calendar?

The calendar the system should refer to when it reschedules a repeating notification.

var region: CLRegion?

The geographic region that triggers the notification.

var regionTriggersOnce: Bool

A Boolean value indicating whether crossing a geographic region boundary delivers only one notification.

### Composing the alert

var alertBody: String?

The message displayed in the notification alert.

var alertAction: String?

The title of the action button or slider.

var alertTitle: String?

A short description of the reason for the alert.

var hasAction: Bool

A Boolean value that controls whether the notification shows or hides the alert action.

var alertLaunchImage: String?

Identifies the image used as the launch image when the user taps (or slides) the action button (or slider).

var category: String?

The name of a group of actions to display in the alert.

### Configuring other parts of the notification

var applicationIconBadgeNumber: Int

The number to display as the app’s icon badge.

var soundName: String?

The name of the file containing the sound to play when an alert is displayed.

var userInfo: [AnyHashable : Any]?

A dictionary for passing custom information to the notified app.

### Constants

Notification sound

The default system sound for local notifications.

### Initializers

init()

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
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

