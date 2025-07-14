

- Foundation
- NSUserNotification
-  activationType Deprecated

Instance Property

# activationType

Specifies what caused a user notification to occur.

macOS 10.8–11.0Deprecated

``` source
var activationType: NSUserNotification.ActivationType { get }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

This property specifies why the user notification was sent to to the NSUserNotificationCenterDelegate method userNotificationCenter(_:didActivate:). The supported values are described in NSUserNotification.ActivationType.

## See Also

### User Notification Activation Method

var additionalActivationAction: NSUserNotificationAction?

An additional action selected by the user.

Deprecated

var additionalActions: [NSUserNotificationAction]?

The actions that can be taken on a notification in addition to the default action.

Deprecated

