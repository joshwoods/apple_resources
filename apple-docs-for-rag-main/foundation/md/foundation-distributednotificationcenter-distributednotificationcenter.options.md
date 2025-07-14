

- Foundation
- DistributedNotificationCenter
-  DistributedNotificationCenter.Options 

Structure

# DistributedNotificationCenter.Options

These constants specify the behavior of notifications posted using the postNotificationName(_:object:userInfo:options:) method.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct Options
```

## Topics

### Constants

static var deliverImmediately: DistributedNotificationCenter.Options

static var postToAllSessions: DistributedNotificationCenter.Options

### Constants

let NSNotificationDeliverImmediately: DistributedNotificationCenter.Options

When set, the notification is delivered immediately to all observers, regardless of their suspension behavior or suspension state. When not set, allows the normal suspension behavior of notification observers to take place.

let NSNotificationPostToAllSessions: DistributedNotificationCenter.Options

When set, the notification is posted to all sessions. When not set, the notification is sent only to applications within the same login session as the posting task.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

struct CenterType

This constant specifies the notification center type.

enum SuspensionBehavior

These constants specify the types of notification delivery suspension behaviors.

