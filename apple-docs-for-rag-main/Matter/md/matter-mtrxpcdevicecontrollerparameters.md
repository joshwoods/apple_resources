

- Matter
-  MTRXPCDeviceControllerParameters 

Class

# MTRXPCDeviceControllerParameters

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
class MTRXPCDeviceControllerParameters
```

## Topics

### Initializers

init(xpConnectionBlock: () -> NSXPCConnection, uniqueIdentifier: UUID)

A controller created from this way will connect to a remote instance of an MTRDeviceController loaded in an XPC Service

### Instance Properties

var uniqueIdentifier: UUID

var xpcConnectionBlock: () -> NSXPCConnection

## Relationships

### Inherits From

- MTRDeviceControllerAbstractParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

