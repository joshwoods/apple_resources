

- Foundation
- NSUserNotificationCenterDelegate
-  userNotificationCenter(\_:shouldPresent:) Deprecated

Instance Method

# userNotificationCenter(\_:shouldPresent:)

Sent to the delegate when the user notification center has decided not to present your notification.

macOS 10.8–11.0Deprecated

``` source
optional func userNotificationCenter(
    _ center: NSUserNotificationCenter,
    shouldPresent notification: NSUserNotification
) -> Bool
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Parameters 

`center`  

The user notification center.

`notification`  

The user notification object.

## Return Value

true if the user notification should be displayed regardless; false otherwise.

