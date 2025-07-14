

- CloudKit
- CKNotification
-  CKNotification.NotificationType 

Enumeration

# CKNotification.NotificationType

Constants that indicate the type of event that generates the push notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
enum NotificationType
```

## Topics

### Notification Types

case query

A notification that CloudKit generates from a query subscription’s predicate.

case database

A notification that CloudKit generates when the contents of a database change.

case recordZone

A notification that CloudKit generates when the contents of a record zone change.

case readNotification

A notification that your app marks as read.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying the Notification

var notificationID: CKNotification.ID?

The notification’s ID.

class ID

An object that uniquely identifies a push notification that a container sends.

var notificationType: CKNotification.NotificationType

The type of event that generates the notification.

var containerIdentifier: String?

The ID of the container with the content that triggers the notification.

