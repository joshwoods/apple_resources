

- IOBluetooth
-  BluetoothHCISetupSynchronousConnectionParams 

Structure

# BluetoothHCISetupSynchronousConnectionParams

macOS

``` source
struct BluetoothHCISetupSynchronousConnectionParams
```

## Topics

### Initializers

init()

init(transmitBandwidth: UInt32, receiveBandwidth: UInt32, maxLatency: UInt16, voiceSetting: UInt16, retransmissionEffort: UInt8, packetType: UInt16)

### Instance Properties

var maxLatency: UInt16

var packetType: UInt16

var receiveBandwidth: UInt32

var retransmissionEffort: UInt8

var transmitBandwidth: UInt32

var voiceSetting: UInt16

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

