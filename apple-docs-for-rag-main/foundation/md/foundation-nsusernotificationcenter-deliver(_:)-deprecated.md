

- Foundation
- NSUserNotificationCenter
-  deliver(\_:) Deprecated

Instance Method

# deliver(\_:)

Deliver the specified user notification.

macOS 10.8–11.0Deprecated

``` source
func deliver(_ notification: NSUserNotification)
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Parameters 

`notification`  

The user notification.

## Discussion

The notification will be presented to the user (subject to the user’s preferences). The isPresented property of the NSUserNotification object will always be set to true if a notification is delivered using this method.

## See Also

### Related Documentation

func removeScheduledNotification(NSUserNotification)

Removes the specified user notification for the scheduled notifications.

Deprecated

### Managing the Delivered Notifications

var deliveredNotifications: [NSUserNotification]

An array of all user notifications delivered to the notification center.

Deprecated

func removeDeliveredNotification(NSUserNotification)

Remove a delivered user notification from the user notification center.

Deprecated

func removeAllDeliveredNotifications()

Remove all delivered user notifications from the user notification center.

Deprecated

