

- IOUSBHost
-  IOUSBHostCIPortStateMachine 

Class

# IOUSBHostCIPortStateMachine

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostCIPortStateMachine
```

## Topics

### Instance Properties

var connected: Bool

var controllerInterface: IOUSBHostControllerInterface

var linkState: IOUSBHostCILinkState

var overcurrent: Bool

var portNumber: Int

var portState: IOUSBHostCIPortState

var portStatus: IOUSBHostCIPortStatus

var powered: Bool

var speed: IOUSBHostCIDeviceSpeed

### Instance Methods

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

func updateLinkState(IOUSBHostCILinkState, speed: IOUSBHostCIDeviceSpeed, inhibitLinkStateChange: Bool) throws

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

class IOUSBHostCIControllerStateMachine

class IOUSBHostCIDeviceStateMachine

class IOUSBHostCIEndpointStateMachine

class IOUSBHostControllerInterface

