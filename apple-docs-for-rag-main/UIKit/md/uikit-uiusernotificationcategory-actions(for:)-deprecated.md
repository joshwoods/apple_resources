

- UIKit
- UIUserNotificationCategory
-  actions(for:) Deprecated

Instance Method

# actions(for:)

Returns the actions to be displayed for the given notification context.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func actions(for context: UIUserNotificationActionContext) -> [UIUserNotificationAction]?
```

## Parameters 

`context`  

The context in which the notification is displayed. Notifications can have a default context or a minimal context depending on whether the notification was just delivered or the user is looking at it in more detail.

## Return Value

An array of UIUserNotificationAction objects to be displayed in the specified context. The order of the objects in the array represents the order that they are displayed in the resulting notification.

## Discussion

This method returns the actions associated with the specified display context. To set the actions for a given context, you must create a UIMutableUserNotificationCategory object and use its setActions:forContext: method to specify your actions.

## See Also

### Getting the group configuration

var identifier: String?

The name of the action group.

Deprecated

