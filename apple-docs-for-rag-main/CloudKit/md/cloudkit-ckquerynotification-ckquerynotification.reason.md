

- CloudKit
- CKQueryNotification
-  CKQueryNotification.Reason 

Enumeration

# CKQueryNotification.Reason

Constants that indicate the event that triggers the notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
enum Reason
```

## Topics

### Constants

case recordCreated

A notification that indicates the creation of a record matching the subscription’s predicate.

case recordUpdated

A notification that indicates the update of a record matching the subscription’s predicate.

case recordDeleted

A notification that indicates the deletion of a record matching the subscription’s predicate.

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

### Getting the Notification Attributes

var queryNotificationReason: CKQueryNotification.Reason

The event that triggers the push notification.

