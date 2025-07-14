

- IOBluetooth
-  BluetoothHCIEventLEConnectionCompleteResults 

Structure

# BluetoothHCIEventLEConnectionCompleteResults

macOS

``` source
struct BluetoothHCIEventLEConnectionCompleteResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, role: UInt8, peerAddressType: UInt8, peerAddress: BluetoothDeviceAddress, connInterval: UInt16, connLatency: UInt16, supervisionTimeout: UInt16, masterClockAccuracy: UInt8)

### Instance Properties

var connInterval: UInt16

var connLatency: UInt16

var connectionHandle: BluetoothConnectionHandle

var masterClockAccuracy: UInt8

var peerAddress: BluetoothDeviceAddress

var peerAddressType: UInt8

var role: UInt8

var supervisionTimeout: UInt16

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

