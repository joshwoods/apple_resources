

- User Notifications
- UNNotificationContent
-  categoryIdentifier 

Instance Property

# categoryIdentifier

The identifier of the notification’s category.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var categoryIdentifier: String { get }
```

## Discussion

Use notification types to distinguish between the different types of notifications your app supports. You use this support primarily to create actionable notifications with custom action buttons, and to redirect your notifications through either your notification service app extension or your notification content app extension.

For remote notifications, the system sets this property to the value of the `category` key in the `aps` dictionary.

## See Also

### Retrieving group information

var threadIdentifier: String

The identifier that groups related notifications.

var summaryArgument: String

The text the system adds to the notification summary to provide additional context.

Deprecated

var summaryArgumentCount: Int

The number the system adds to the notification summary when the notification represents multiple items.

Deprecated

