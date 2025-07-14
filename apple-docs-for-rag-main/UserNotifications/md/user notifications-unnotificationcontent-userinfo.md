

- User Notifications
- UNNotificationContent
-  userInfo 

Instance Property

# userInfo

The custom data to associate with the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var userInfo: [AnyHashable : Any] { get }
```

## Mentioned in 

Declaring your actionable notification types

Generating a remote notification

## Discussion

For remote notifications, this property contains the entire notification payload. For local notifications, you configure the property directly before scheduling the notification.

The keys in this dictionary must be property-list types—that’s, they must be types that can be serialized into the property-list format. For information about property-list types, see Property List Programming Guide.

## See Also

### Accessing supplementary content

var attachments: [UNNotificationAttachment]

The visual and audio attachments to display alongside the notification’s main content.

