

- Foundation
- NSUserNotificationCenter
-  removeScheduledNotification(\_:) Deprecated

Instance Method

# removeScheduledNotification(\_:)

Removes the specified user notification for the scheduled notifications.

macOS 10.8–11.0Deprecated

``` source
func removeScheduledNotification(_ notification: NSUserNotification)
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Parameters 

`notification`  

The user notification.

## Discussion

If the user notification’s deliveryDate occurs before the cancellation finishes, the notification may still be delivered.

If the notification is not in the scheduled list, nothing happens.

## See Also

### Managing the Scheduled Notification Queue

func scheduleNotification(NSUserNotification)

Schedules the specified user notification.

Deprecated

var scheduledNotifications: [NSUserNotification]

Specifies an array of scheduled user notifications that have not yet been delivered.

Deprecated

