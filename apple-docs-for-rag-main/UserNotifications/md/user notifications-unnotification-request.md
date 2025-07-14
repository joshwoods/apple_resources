

- User Notifications
- UNNotification
-  request 

Instance Property

# request

The notification request containing the payload and trigger condition for the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var request: UNNotificationRequest { get }
```

## Discussion

For local notifications, the request object is a copy of the one you originally configured. For remote notifications, the system synthesizes the request object from information received from Apple Push Notification service.

## See Also

### Getting the Notification Details

var date: Date

The delivery date of the notification.

