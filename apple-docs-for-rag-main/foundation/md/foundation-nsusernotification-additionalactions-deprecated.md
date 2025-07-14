

- Foundation
- NSUserNotification
-  additionalActions Deprecated

Instance Property

# additionalActions

The actions that can be taken on a notification in addition to the default action.

macOS 10.10–11.0Deprecated

``` source
var additionalActions: [NSUserNotificationAction]? { get set }
```

## Discussion

This array contains `NSUserNotificationAction` objects that describe the different actions for a notification in addition to the default action described by actionButtonTitle.

## See Also

### Related Documentation

var otherButtonTitle: String

Specifies a custom title for the close button in an alert-style notification.

Deprecated

var actionButtonTitle: String

Specifies the title of the action button displayed in the notification.

Deprecated

### User Notification Activation Method

var activationType: NSUserNotification.ActivationType

Specifies what caused a user notification to occur.

Deprecated

var additionalActivationAction: NSUserNotificationAction?

An additional action selected by the user.

Deprecated

