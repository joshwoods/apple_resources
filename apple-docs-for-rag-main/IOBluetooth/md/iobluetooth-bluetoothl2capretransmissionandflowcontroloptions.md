

- IOBluetooth
-  BluetoothL2CAPRetransmissionAndFlowControlOptions 

Structure

# BluetoothL2CAPRetransmissionAndFlowControlOptions

macOS

``` source
struct BluetoothL2CAPRetransmissionAndFlowControlOptions
```

## Topics

### Initializers

init()

init(flags: UInt8, txWindowSize: UInt8, maxTransmit: UInt8, retransmissionTimeout: UInt16, monitorTimeout: UInt16, maxPDUPayloadSize: UInt16)

### Instance Properties

var flags: UInt8

var maxPDUPayloadSize: UInt16

var maxTransmit: UInt8

var monitorTimeout: UInt16

var retransmissionTimeout: UInt16

var txWindowSize: UInt8

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

