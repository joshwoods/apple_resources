

- Foundation
- NSUserNotificationCenter
-  scheduledNotifications Deprecated

Instance Property

# scheduledNotifications

Specifies an array of scheduled user notifications that have not yet been delivered.

macOS 10.8–11.0Deprecated

``` source
var scheduledNotifications: [NSUserNotification] { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

Newly scheduled notifications are added to the end of the array. You may also bulk-schedule notifications by setting this array. Bulk setting new scheduled notifications unschedules existing notifications.

Note

The scheduled user notification could be changing to a delivered notification at the time you are calling this method. and if that case the user notification will still be delivered.

## See Also

### Managing the Scheduled Notification Queue

func scheduleNotification(NSUserNotification)

Schedules the specified user notification.

Deprecated

func removeScheduledNotification(NSUserNotification)

Removes the specified user notification for the scheduled notifications.

Deprecated

