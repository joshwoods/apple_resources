

- IOUSBHost
-  IOUSBHostCIDeviceStateMachine 

Class

# IOUSBHostCIDeviceStateMachine

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostCIDeviceStateMachine
```

## Topics

### Instance Properties

var completeRoute: Int

var controllerInterface: IOUSBHostControllerInterface

var deviceAddress: Int

var deviceState: IOUSBHostCIDeviceState

### Instance Methods

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, deviceAddress: Int) throws

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

class IOUSBHostCIEndpointStateMachine

class IOUSBHostCIPortStateMachine

class IOUSBHostControllerInterface

