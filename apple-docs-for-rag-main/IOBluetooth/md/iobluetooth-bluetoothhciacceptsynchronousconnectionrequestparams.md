

- IOBluetooth
-  BluetoothHCIAcceptSynchronousConnectionRequestParams 

Structure

# BluetoothHCIAcceptSynchronousConnectionRequestParams

macOS

``` source
struct BluetoothHCIAcceptSynchronousConnectionRequestParams
```

## Topics

### Initializers

init()

init(transmitBandwidth: UInt32, receiveBandwidth: UInt32, maxLatency: UInt16, contentFormat: UInt16, retransmissionEffort: UInt8, packetType: UInt16)

### Instance Properties

var contentFormat: UInt16

var maxLatency: UInt16

var packetType: UInt16

var receiveBandwidth: UInt32

var retransmissionEffort: UInt8

var transmitBandwidth: UInt32

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

