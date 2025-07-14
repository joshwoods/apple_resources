

- CloudKit
- CKNotification
-  notificationType 

Instance Property

# notificationType

The type of event that generates the notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var notificationType: CKNotification.NotificationType { get }
```

## Discussion

Different notification types correspond to different subclasses of `CKNotification`, so you can use the value in this property to determine how to handle the notification data.

## See Also

### Identifying the Notification

var notificationID: CKNotification.ID?

The notification’s ID.

class ID

An object that uniquely identifies a push notification that a container sends.

enum NotificationType

Constants that indicate the type of event that generates the push notification.

var containerIdentifier: String?

The ID of the container with the content that triggers the notification.

