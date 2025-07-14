

- IOUSBHost
-  IOUSBHostCIControllerStateMachine 

Class

# IOUSBHostCIControllerStateMachine

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostCIControllerStateMachine
```

## Topics

### Instance Properties

var controllerInterface: IOUSBHostControllerInterface

var controllerState: IOUSBHostCIControllerState

### Instance Methods

func enqueueUpdatedFrame(UInt64, timestamp: UInt64) throws

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, frame: UInt64, timestamp: UInt64) throws

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class IOUSBHostCIDeviceStateMachine

class IOUSBHostCIEndpointStateMachine

class IOUSBHostCIPortStateMachine

class IOUSBHostControllerInterface

