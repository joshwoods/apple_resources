

- IOBluetooth
-  BluetoothHCIEventSynchronousConnectionChangedResults 

Structure

# BluetoothHCIEventSynchronousConnectionChangedResults

macOS

``` source
struct BluetoothHCIEventSynchronousConnectionChangedResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, transmissionInterval: UInt8, retransmissionWindow: UInt8, receivePacketLength: UInt16, transmitPacketLength: UInt16)

### Instance Properties

var connectionHandle: BluetoothConnectionHandle

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

