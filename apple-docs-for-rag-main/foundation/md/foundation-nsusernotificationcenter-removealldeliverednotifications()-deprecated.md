

- Foundation
- NSUserNotificationCenter
-  removeAllDeliveredNotifications() Deprecated

Instance Method

# removeAllDeliveredNotifications()

Remove all delivered user notifications from the user notification center.

macOS 10.8–11.0Deprecated

``` source
func removeAllDeliveredNotifications()
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## See Also

### Managing the Delivered Notifications

func deliver(NSUserNotification)

Deliver the specified user notification.

Deprecated

var deliveredNotifications: [NSUserNotification]

An array of all user notifications delivered to the notification center.

Deprecated

func removeDeliveredNotification(NSUserNotification)

Remove a delivered user notification from the user notification center.

Deprecated

