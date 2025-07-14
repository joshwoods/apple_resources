

- System
- Mach
-  Mach.PortRightError 

Enumeration

# Mach.PortRightError

Possible errors that can be thrown by Mach.Port operations.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
enum PortRightError
```

## Topics

### Operators

static func == (Mach.PortRightError, Mach.PortRightError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case deadName

Returned when an operation cannot be completed, because the Mach port right has become a dead name. This is caused by deallocation of the receive right on the other end.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

