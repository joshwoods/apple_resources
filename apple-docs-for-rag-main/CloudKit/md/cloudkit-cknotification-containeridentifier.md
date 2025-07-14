

- CloudKit
- CKNotification
-  containerIdentifier 

Instance Property

# containerIdentifier

The ID of the container with the content that triggers the notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var containerIdentifier: String? { get }
```

## Discussion

Use this property to determine the location of the changed content.

## See Also

### Identifying the Notification

var notificationID: CKNotification.ID?

The notification’s ID.

class ID

An object that uniquely identifies a push notification that a container sends.

var notificationType: CKNotification.NotificationType

The type of event that generates the notification.

enum NotificationType

Constants that indicate the type of event that generates the push notification.

