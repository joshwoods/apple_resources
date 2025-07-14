

- IOUSBHost
-  IOUSBHostIsochronousTransaction 

Structure

# IOUSBHostIsochronousTransaction

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostIsochronousTransaction
```

## Topics

### Initializers

init()

init(status: IOReturn, requestCount: UInt32, offset: UInt32, completeCount: UInt32, timeStamp: IOUSBHostTime, options: IOUSBHostIsochronousTransactionOptions)

### Instance Properties

var completeCount: UInt32

var offset: UInt32

var options: IOUSBHostIsochronousTransactionOptions

var requestCount: UInt32

var status: IOReturn

var timeStamp: IOUSBHostTime

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

struct IOUSBHostCIMessage

struct IOUSBHostCIMessageStatus

struct IOUSBHostCIMessageType

struct IOUSBHostCIPortState

struct IOUSBHostCIUserClientVersion

struct IOUSBHostIsochronousTransactionOptions

struct IOUSBHostIsochronousTransferOptions

struct IOUSBHostObjectDestroyOptions

