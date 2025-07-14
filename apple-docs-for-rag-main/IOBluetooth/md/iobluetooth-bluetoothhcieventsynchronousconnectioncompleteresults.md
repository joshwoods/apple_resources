

- IOBluetooth
-  BluetoothHCIEventSynchronousConnectionCompleteResults 

Structure

# BluetoothHCIEventSynchronousConnectionCompleteResults

macOS

``` source
struct BluetoothHCIEventSynchronousConnectionCompleteResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, deviceAddress: BluetoothDeviceAddress, linkType: BluetoothLinkType, transmissionInterval: UInt8, retransmissionWindow: UInt8, receivePacketLength: UInt16, transmitPacketLength: UInt16, airMode: BluetoothAirMode)

### Instance Properties

var airMode: BluetoothAirMode

var connectionHandle: BluetoothConnectionHandle

var deviceAddress: BluetoothDeviceAddress

var linkType: BluetoothLinkType

var receivePacketLength: UInt16

var retransmissionWindow: UInt8

var transmissionInterval: UInt8

var transmitPacketLength: UInt16

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct BluetoothAFHHostChannelClassification

struct BluetoothAFHResults

struct BluetoothAMPCommandRejectReason

struct BluetoothAMPCreatePhysicalLinkResponseStatus

struct BluetoothAMPDisconnectPhysicalLinkResponseStatus

struct BluetoothAMPDiscoverResponseControllerStatus

struct BluetoothAMPGetAssocResponseStatus

struct BluetoothAMPGetInfoResponseStatus

struct BluetoothAMPManagerCode

struct BluetoothAuthenticationRequirementsValues

struct BluetoothCompanyIdentifers

struct BluetoothDeviceAddress

struct BluetoothEnhancedSynchronousConnectionInfo

struct BluetoothEventFilterCondition

struct BluetoothFeatureBits

