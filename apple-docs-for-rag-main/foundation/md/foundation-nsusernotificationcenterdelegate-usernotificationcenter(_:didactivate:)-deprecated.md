

- Foundation
- NSUserNotificationCenterDelegate
-  userNotificationCenter(\_:didActivate:) Deprecated

Instance Method

# userNotificationCenter(\_:didActivate:)

Sent to the delegate when a user clicks on a user notification presented by the user notification center.

macOS 10.8–11.0Deprecated

``` source
optional func userNotificationCenter(
    _ center: NSUserNotificationCenter,
    didActivate notification: NSUserNotification
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

This would be a good time to take action in response to user interacting with a specific notification.

To take an action when your application is launched as a result of a user clicking on a notification, be sure to implement the applicationDidFinishLaunching(_:) method in the application class that implements the NSApplicationDelegate protocol. The notification parameter to that method has a `userInfo` dictionary, and if that dictionary has the `NSApplicationLaunchUserNotificationKey` key. The value of that key is the NSUserNotification object that caused the application to launch. The `NSUserNotification` object is delivered to the `NSApplication` delegate because that message will be sent before your application has a chance to set a delegate for the `NSUserNotificationCenter`.

## See Also

### User Notification Delivery Information

func userNotificationCenter(NSUserNotificationCenter, didDeliver: NSUserNotification)

Sent to the delegate when a notification delivery date has arrived.

Deprecated

