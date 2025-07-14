

- EventKit
-  EKEntityMask 

Structure

# EKEntityMask

A bitmask of `EKEntityType` for specifying multiple entities at once.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct EKEntityMask
```

## Topics

### Initializers

init(rawValue: UInt)

Creates an entity mask with the specified raw value.

### Constants

static var event: EKEntityMask

Represents an event.

static var reminder: EKEntityMask

Represents a reminder.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

