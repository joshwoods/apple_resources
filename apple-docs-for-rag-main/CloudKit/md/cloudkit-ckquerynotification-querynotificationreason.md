

- CloudKit
- CKQueryNotification
-  queryNotificationReason 

Instance Property

# queryNotificationReason

The event that triggers the push notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var queryNotificationReason: CKQueryNotification.Reason { get }
```

## Discussion

Subscription notifications result from the creation, deletion, or updating of a single record. The record in question must match the subscription’s predicate for an event to trigger.

## See Also

### Getting the Notification Attributes

enum Reason

Constants that indicate the event that triggers the notification.

