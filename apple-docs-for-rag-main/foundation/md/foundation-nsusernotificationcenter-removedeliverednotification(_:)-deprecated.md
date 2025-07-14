

- Foundation
- NSUserNotificationCenter
-  removeDeliveredNotification(\_:) Deprecated

Instance Method

# removeDeliveredNotification(\_:)

Remove a delivered user notification from the user notification center.

macOS 10.8–11.0Deprecated

``` source
func removeDeliveredNotification(_ notification: NSUserNotification)
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Parameters 

`notification`  

The user notification.

## Discussion

If the user notification is not in deliveredNotifications, nothing happens.

## See Also

### Managing the Delivered Notifications

func deliver(NSUserNotification)

Deliver the specified user notification.

Deprecated

var deliveredNotifications: [NSUserNotification]

An array of all user notifications delivered to the notification center.

Deprecated

func removeAllDeliveredNotifications()

Remove all delivered user notifications from the user notification center.

Deprecated

