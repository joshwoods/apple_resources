

- IOUSBHost
-  IOUSBHostCIEndpointStateMachine 

Class

# IOUSBHostCIEndpointStateMachine

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostCIEndpointStateMachine
```

## Topics

### Instance Properties

var controllerInterface: IOUSBHostControllerInterface

var currentTransferMessage: UnsafePointer&lt;IOUSBHostCIMessage>

var deviceAddress: Int

var endpointAddress: Int

var endpointState: IOUSBHostCIEndpointState

### Instance Methods

func enqueueTransferCompletion(for: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, transferLength: Int) throws

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func processDoorbell(IOUSBHostCIDoorbell) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

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

class IOUSBHostCIPortStateMachine

class IOUSBHostControllerInterface

