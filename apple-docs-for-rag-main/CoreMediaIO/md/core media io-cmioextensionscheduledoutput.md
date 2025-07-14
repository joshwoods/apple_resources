

- Core Media I/O
-  CMIOExtensionScheduledOutput 

Class

# CMIOExtensionScheduledOutput

An object that represents scheduled output.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionScheduledOutput
```

## Topics

### Creating a Scheduled Output

init(sequenceNumber: UInt64, hostTimeInNanoseconds: UInt64)

Creates a scheduled output object.

### Inspecting the Output

var sequenceNumber: UInt64

The buffer sequence number that was output.

var hostTimeInNanoseconds: UInt64

The host time in nanoseconds when the buffer was output.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Managing Scheduled Output

func notifyScheduledOutputChanged(CMIOExtensionScheduledOutput)

Notifies clients when a particular buffer is output.

