

- Foundation
-  NSUserNotificationCenter Deprecated

Class

# NSUserNotificationCenter

An object that delivers notifications from apps to the user.

macOS 10.8–11.0Deprecated

``` source
class NSUserNotificationCenter
```

Deprecated

Use the User Notifications framework instead.

## Overview

When a user notification’s delivery date has been reached, or it’s manually delivered, the notification center may display the notification to the user. The user notification center reserves the right to decide if a delivered user notification is presented to the user. For example, it may suppress the notification if the application is already frontmost (the delegate can override this action). The application can check the result of this decision by examining the isPresented property of a delivered user notification.

NSUserNotification instances the `NSUserNotificationCenter` are tracking will be in one of two states: scheduled or delivered. A scheduled user notification has a deliveryDate. On that delivery date, the notification will move from being scheduled to being delivered. Note that the user notification may be displayed later than the delivery date depending on many factors.

A delivered user notification has an actualDeliveryDate. That’s the date when it moved from being scheduled to delivered, or when it was manually delivered using the deliver(_:) method.

The application and the user notification center are both ultimately subject to the user’s preferences. If the user decides to hide all alerts from your application, the `presented` property will still behave as above, but the user won’t see any animation or hear any sound.

The NSUserNotificationCenterDelegate provides more information about the delivered user notification and allows forcing the display of a user notification even if the application is frontmost.

Note

It the user wakes more than 15 minutes after a scheduled notification is scheduled to fire, it’s discarded. If the notification repeats with an interval less than 15 minutes, then it expires in 1 minute. Expired notifications are just discarded, unless they repeat, in which case, they stay in the scheduled list and just fire again later.

Important

Many of the NSUserNotificationCenter class’s methods involve talking to a server process, so calling them repeatedly can have a negative effect on performance.

### Threading Information

The `NSUserNotificationCenter` class and the NSUserNotification class are both thread safe.

## Topics

### Creating the Default User Notification Center

class var `default`: NSUserNotificationCenter

Returns the default user notification center.

### Managing the Scheduled Notification Queue

func scheduleNotification(NSUserNotification)

Schedules the specified user notification.

var scheduledNotifications: [NSUserNotification]

Specifies an array of scheduled user notifications that have not yet been delivered.

func removeScheduledNotification(NSUserNotification)

Removes the specified user notification for the scheduled notifications.

### Managing the Delivered Notifications

func deliver(NSUserNotification)

Deliver the specified user notification.

var deliveredNotifications: [NSUserNotification]

An array of all user notifications delivered to the notification center.

func removeDeliveredNotification(NSUserNotification)

Remove a delivered user notification from the user notification center.

func removeAllDeliveredNotifications()

Remove all delivered user notifications from the user notification center.

### Getting and Setting the Delegate

var delegate: (any NSUserNotificationCenterDelegate)?

Specifies the notification center delegate.

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

## See Also

### User Notifications

class NSUserNotification

A notification that can be scheduled for display in the notification center.

Deprecated

class NSUserNotificationAction

An action that the user can take in response to receiving a notification.

Deprecated

protocol NSUserNotificationCenterDelegate

An interface that enables customizing the behavior of the default notification center.

