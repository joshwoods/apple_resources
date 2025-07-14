

- Foundation
-  NSUserNotificationCenterDelegate 

Protocol

# NSUserNotificationCenterDelegate

An interface that enables customizing the behavior of the default notification center.

Mac Catalyst 13.0+macOS 10.0+

``` source
protocol NSUserNotificationCenterDelegate : NSObjectProtocol
```

## Topics

### User Notification Delivery Information

func userNotificationCenter(NSUserNotificationCenter, didDeliver: NSUserNotification)

Sent to the delegate when a notification delivery date has arrived.

Deprecated

func userNotificationCenter(NSUserNotificationCenter, didActivate: NSUserNotification)

Sent to the delegate when a user clicks on a user notification presented by the user notification center.

Deprecated

### User Notification Display Override

func userNotificationCenter(NSUserNotificationCenter, shouldPresent: NSUserNotification) -> Bool

Sent to the delegate when the user notification center has decided not to present your notification.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### User Notifications

class NSUserNotification

A notification that can be scheduled for display in the notification center.

Deprecated

class NSUserNotificationAction

An action that the user can take in response to receiving a notification.

Deprecated

class NSUserNotificationCenter

An object that delivers notifications from apps to the user.

Deprecated

