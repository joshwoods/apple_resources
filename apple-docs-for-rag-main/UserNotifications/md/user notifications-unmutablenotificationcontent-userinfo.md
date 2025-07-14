

- User Notifications
- UNMutableNotificationContent
-  userInfo 

Instance Property

# userInfo

The custom data to associate with the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var userInfo: [AnyHashable : Any] { get set }
```

## Mentioned in 

Declaring your actionable notification types

## Discussion

Use this property to associate custom information with the notification. The contents of the dictionary aren’t seen by the user, but are accessible to your app or to any notification-related app extensions.

The keys in this dictionary must be types that can be serialized into the property-list format. For information about property-list types, see Property List Programming Guide.

## See Also

### Providing supplementary content

var attachments: [UNNotificationAttachment]

The visual and audio attachments to display alongside the notification’s main content.

