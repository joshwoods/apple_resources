

- IOUSBHost
-  IOUSBHostCIMessage 

Structure

# IOUSBHostCIMessage

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostCIMessage
```

## Topics

### Initializers

init()

init(control: UInt32, data0: UInt32, data1: UInt64)

### Instance Properties

var control: UInt32

var data0: UInt32

var data1: UInt64

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct IOUSBHostCIControllerState

struct IOUSBHostCIDeviceSpeed

struct IOUSBHostCIDeviceState

struct IOUSBHostCIEndpointState

struct IOUSBHostCIExceptionType

struct IOUSBHostCILinkState

struct IOUSBHostCIMessageStatus

struct IOUSBHostCIMessageType

struct IOUSBHostCIPortState

struct IOUSBHostCIUserClientVersion

struct IOUSBHostIsochronousTransaction

struct IOUSBHostIsochronousTransactionOptions

struct IOUSBHostIsochronousTransferOptions

struct IOUSBHostObjectDestroyOptions

