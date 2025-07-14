

- Foundation
- DistributedNotificationCenter
-  DistributedNotificationCenter.CenterType 

Structure

# DistributedNotificationCenter.CenterType

This constant specifies the notification center type.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct CenterType
```

## Topics

### Type Properties

static let localNotificationCenterType: DistributedNotificationCenter.CenterType

Distributes notifications to all tasks on the sender’s computer.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct Options

These constants specify the behavior of notifications posted using the postNotificationName(_:object:userInfo:options:) method.

enum SuspensionBehavior

These constants specify the types of notification delivery suspension behaviors.

