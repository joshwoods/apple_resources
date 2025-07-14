

- User Notifications
- UNNotificationContent
-  threadIdentifier 

Instance Property

# threadIdentifier

The identifier that groups related notifications.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var threadIdentifier: String { get }
```

## Discussion

For remote notifications, the system sets this property to the value of the `thread-id` key in the `aps` dictionary.

## See Also

### Retrieving group information

var categoryIdentifier: String

The identifier of the notification’s category.

var summaryArgument: String

The text the system adds to the notification summary to provide additional context.

Deprecated

var summaryArgumentCount: Int

The number the system adds to the notification summary when the notification represents multiple items.

Deprecated

