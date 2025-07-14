

- Foundation
- NSUserNotificationCenterDelegate
-  userNotificationCenter(\_:didDeliver:) Deprecated

Instance Method

# userNotificationCenter(\_:didDeliver:)

Sent to the delegate when a notification delivery date has arrived.

macOS 10.8–11.0Deprecated

``` source
optional func userNotificationCenter(
    _ center: NSUserNotificationCenter,
    didDeliver notification: NSUserNotification
)
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Parameters 

`center`  

The user notification center.

`notification`  

The user notification object.

## Discussion

This method is always called, regardless of your application state and even if you deliver the user notification yourself using deliver(_:).

This delegate method is invoked before the userNotificationCenter(_:shouldPresent:) delegate method.

## See Also

### User Notification Delivery Information

func userNotificationCenter(NSUserNotificationCenter, didActivate: NSUserNotification)

Sent to the delegate when a user clicks on a user notification presented by the user notification center.

Deprecated

