

- IOBluetooth
-  IOBluetoothL2CAPChannelEventType 

Structure

# IOBluetoothL2CAPChannelEventType

macOS

``` source
struct IOBluetoothL2CAPChannelEventType
```

## Topics

### Constants

var kIOBluetoothL2CAPChannelEventTypeClosed: IOBluetoothL2CAPChannelEventType

var kIOBluetoothL2CAPChannelEventTypeData: IOBluetoothL2CAPChannelEventType

var kIOBluetoothL2CAPChannelEventTypeOpenComplete: IOBluetoothL2CAPChannelEventType

var kIOBluetoothL2CAPChannelEventTypeQueueSpaceAvailable: IOBluetoothL2CAPChannelEventType

var kIOBluetoothL2CAPChannelEventTypeReconfigured: IOBluetoothL2CAPChannelEventType

var kIOBluetoothL2CAPChannelEventTypeWriteComplete: IOBluetoothL2CAPChannelEventType

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

struct BluetoothAMPCommandRejectReason

struct BluetoothAMPCreatePhysicalLinkResponseStatus

struct BluetoothAMPDisconnectPhysicalLinkResponseStatus

struct BluetoothAMPDiscoverResponseControllerStatus

struct BluetoothAMPGetAssocResponseStatus

struct BluetoothAMPGetInfoResponseStatus

struct BluetoothAMPManagerCode

struct BluetoothHCIPowerState

struct BluetoothL2CAPCommandCode

struct BluetoothL2CAPCommandRejectReason

struct BluetoothL2CAPConfigurationOption

struct BluetoothL2CAPConfigurationResult

struct BluetoothL2CAPConfigurationRetransmissionAndFlowControlFlags

struct BluetoothL2CAPConnectionResult

struct BluetoothL2CAPConnectionStatus

