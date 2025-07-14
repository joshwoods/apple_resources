

- IOBluetooth
-  BluetoothSynchronousConnectionInfo 

Structure

# BluetoothSynchronousConnectionInfo

macOS

``` source
struct BluetoothSynchronousConnectionInfo
```

## Topics

### Initializers

init()

init(transmitBandWidth: BluetoothHCITransmitBandwidth, receiveBandWidth: BluetoothHCIReceiveBandwidth, maxLatency: BluetoothHCIMaxLatency, voiceSetting: BluetoothHCIVoiceSetting, retransmissionEffort: BluetoothHCIRetransmissionEffort, packetType: BluetoothPacketType)

### Instance Properties

var maxLatency: BluetoothHCIMaxLatency

var packetType: BluetoothPacketType

var receiveBandWidth: BluetoothHCIReceiveBandwidth

var retransmissionEffort: BluetoothHCIRetransmissionEffort

var transmitBandWidth: BluetoothHCITransmitBandwidth

var voiceSetting: BluetoothHCIVoiceSetting

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

