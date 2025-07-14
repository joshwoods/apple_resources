

- IOBluetooth
-  BluetoothHCIEventSniffSubratingResults 

Structure

# BluetoothHCIEventSniffSubratingResults

macOS

``` source
struct BluetoothHCIEventSniffSubratingResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, maxTransmitLatency: UInt16, maxReceiveLatency: UInt16, minRemoteTimeout: UInt16, minLocalTimeout: UInt16)

### Instance Properties

var connectionHandle: BluetoothConnectionHandle

var maxReceiveLatency: UInt16

var maxTransmitLatency: UInt16

var minLocalTimeout: UInt16

var minRemoteTimeout: UInt16

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

