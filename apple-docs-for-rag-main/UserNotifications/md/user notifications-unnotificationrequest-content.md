

- User Notifications
- UNNotificationRequest
-  content 

Instance Property

# content

The content associated with the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var content: UNNotificationContent { get }
```

## Discussion

Use this property to access the contents of the notification.

## See Also

### Getting the Request Details

var identifier: String

The unique identifier for this notification request.

var trigger: UNNotificationTrigger?

The conditions that trigger the delivery of the notification.

