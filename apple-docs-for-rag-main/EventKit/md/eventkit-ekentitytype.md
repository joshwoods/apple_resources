

- EventKit
-  EKEntityType 

Enumeration

# EKEntityType

The type of entities allowed for a source.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKEntityType
```

## Topics

### Specifying Multiple Entities

struct EKEntityMask

A bitmask of `EKEntityType` for specifying multiple entities at once.

### Constants

case event

Represents an event.

case reminder

Represents a reminder.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

