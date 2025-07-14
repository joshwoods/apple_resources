

- Foundation
- NSUserNotificationCenter
-  scheduleNotification(\_:) Deprecated

Instance Method

# scheduleNotification(\_:)

Schedules the specified user notification.

macOS 10.8–11.0Deprecated

``` source
func scheduleNotification(_ notification: NSUserNotification)
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Parameters 

`notification`  

The user notification.

## Discussion

Scheduled notifications are added to the end of the notification queue.

## See Also

### Related Documentation

func deliver(NSUserNotification)

Deliver the specified user notification.

Deprecated

### Managing the Scheduled Notification Queue

var scheduledNotifications: [NSUserNotification]

Specifies an array of scheduled user notifications that have not yet been delivered.

Deprecated

func removeScheduledNotification(NSUserNotification)

Removes the specified user notification for the scheduled notifications.

Deprecated

