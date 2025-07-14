

- IOUSBHost
-  IOUSBHostControllerInterface 

Class

# IOUSBHostControllerInterface

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostControllerInterface
```

## Topics

### Instance Properties

var capabilities: UnsafePointer&lt;IOUSBHostCIMessage>

var controllerStateMachine: IOUSBHostCIControllerStateMachine

var interruptRateHz: Int

var queue: dispatch_queue_t

var uuid: UUID

### Instance Methods

func capabilities(forPort: Int) -> UnsafePointer&lt;IOUSBHostCIMessage>

func description(for: UnsafePointer&lt;IOUSBHostCIMessage>) -> String

func destroy()

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>, expedite: Bool) throws

func enqueueInterrupts(UnsafePointer&lt;IOUSBHostCIMessage>, count: Int) throws

func enqueueInterrupts(UnsafePointer&lt;IOUSBHostCIMessage>, count: Int, expedite: Bool) throws

func getPortStateMachine(forCommand: UnsafePointer&lt;IOUSBHostCIMessage>, error: NSErrorPointer) -> IOUSBHostCIPortStateMachine

func getPortStateMachine(forPort: Int, error: NSErrorPointer) -> IOUSBHostCIPortStateMachine

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

class IOUSBHostCIPortStateMachine

