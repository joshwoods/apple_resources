

- UIKit
- UIUserNotificationCategory
-  identifier Deprecated

Instance Property

# identifier

The name of the action group.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var identifier: String? { get }
```

## Discussion

When generating a notification that includes these custom actions, you must use this string to initialize the notification. For local notifications, assign the string to the category property of the UILocalNotification object. For push notifications, use the string as the value of the `category` key in the push notification’s payload.

## See Also

### Getting the group configuration

func actions(for: UIUserNotificationActionContext) -> [UIUserNotificationAction]?

Returns the actions to be displayed for the given notification context.

Deprecated

