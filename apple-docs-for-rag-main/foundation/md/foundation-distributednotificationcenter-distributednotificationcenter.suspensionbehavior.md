

- Foundation
- DistributedNotificationCenter
-  DistributedNotificationCenter.SuspensionBehavior 

Enumeration

# DistributedNotificationCenter.SuspensionBehavior

These constants specify the types of notification delivery suspension behaviors.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SuspensionBehavior
```

## Topics

### Constants

case drop

The server does not queue any notifications with this name and object until suspended with an argument of false is called.

case coalesce

The server only queues the last notification of the specified name and object; earlier notifications are dropped. In cover methods for which suspension behavior is not an explicit argument, `NSNotificationSuspensionBehaviorCoalesce` is the default.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

case deliverImmediately

case drop

The server does not queue any notifications with this name and object until suspended with an argument of false is called.

case coalesce

The server only queues the last notification of the specified name and object; earlier notifications are dropped. In cover methods for which suspension behavior is not an explicit argument, `NSNotificationSuspensionBehaviorCoalesce` is the default.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

case deliverImmediately

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct Options

These constants specify the behavior of notifications posted using the postNotificationName(_:object:userInfo:options:) method.

struct CenterType

This constant specifies the notification center type.

