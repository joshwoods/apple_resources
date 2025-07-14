

- Foundation
- NSUserNotification
-  additionalActivationAction Deprecated

Instance Property

# additionalActivationAction

An additional action selected by the user.

macOS 10.10–11.0Deprecated

``` source
@NSCopying
var additionalActivationAction: NSUserNotificationAction? { get }
```

## Discussion

This property specifies an additional action selected by the user when the user notification is sent to to the NSUserNotificationCenterDelegate method userNotificationCenter(_:didActivate:). The supported values are described in NSUserNotification.ActivationType.

## See Also

### User Notification Activation Method

var activationType: NSUserNotification.ActivationType

Specifies what caused a user notification to occur.

Deprecated

var additionalActions: [NSUserNotificationAction]?

The actions that can be taken on a notification in addition to the default action.

Deprecated

