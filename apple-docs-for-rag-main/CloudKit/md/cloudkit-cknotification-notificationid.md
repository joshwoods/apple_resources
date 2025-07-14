

- CloudKit
- CKNotification
-  notificationID 

Instance Property

# notificationID

The notification’s ID.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var notificationID: CKNotification.ID? { get }
```

## Discussion

Use this property to differentiate notifications.

## See Also

### Identifying the Notification

class ID

An object that uniquely identifies a push notification that a container sends.

var notificationType: CKNotification.NotificationType

The type of event that generates the notification.

enum NotificationType

Constants that indicate the type of event that generates the push notification.

var containerIdentifier: String?

The ID of the container with the content that triggers the notification.

