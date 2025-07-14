

- Foundation
- NSUserNotificationCenter
-  deliveredNotifications Deprecated

Instance Property

# deliveredNotifications

An array of all user notifications delivered to the notification center.

macOS 10.8–11.0Deprecated

``` source
var deliveredNotifications: [NSUserNotification] { get }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

The number of notifications the user actually sees in the user interface may be less than the size of this array.

Note that these may or may not have been actually presented to the user. See the isPresented property in the NSUserNotification class.

Note

A scheduled user notification that specifies a deliveryRepeatInterval remains in the scheduledNotifications list, even though it has been delivered. The item that goes into the `deliveredNotifications` list is a copy of the user notification item.

## See Also

### Managing the Delivered Notifications

func deliver(NSUserNotification)

Deliver the specified user notification.

Deprecated

func removeDeliveredNotification(NSUserNotification)

Remove a delivered user notification from the user notification center.

Deprecated

func removeAllDeliveredNotifications()

Remove all delivered user notifications from the user notification center.

Deprecated

