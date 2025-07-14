

- UIKit
- UIMutableUserNotificationCategory
-  identifier Deprecated

Instance Property

# identifier

The name of the action group.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var identifier: String? { get set }
```

## Discussion

This property is a writable version of the one declared by the parent class.

When generating a notification that includes these custom actions, you must use this string to initialize the notification. For local notifications, assign the string to the category property of the UILocalNotification object. For push notifications, use the string as the value of the `category` key in the push notification’s payload.

## See Also

### Modifying the action settings

func setActions([UIUserNotificationAction]?, for: UIUserNotificationActionContext)

Sets the actions to display for different alert styles.

Deprecated

