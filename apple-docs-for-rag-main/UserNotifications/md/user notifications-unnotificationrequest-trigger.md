

- User Notifications
- UNNotificationRequest
-  trigger 

Instance Property

# trigger

The conditions that trigger the delivery of the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var trigger: UNNotificationTrigger? { get }
```

## Discussion

For notifications that the system has delivered, use this property to determine what caused the delivery to occur. For remote notifications, this property contains a UNPushNotificationTrigger object. For other notifications, the system sets this type using the trigger condition specified in the original request.

## See Also

### Getting the Request Details

var identifier: String

The unique identifier for this notification request.

var content: UNNotificationContent

The content associated with the notification.

