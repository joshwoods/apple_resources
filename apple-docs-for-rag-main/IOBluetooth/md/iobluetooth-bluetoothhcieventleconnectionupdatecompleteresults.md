

- IOBluetooth
-  BluetoothHCIEventLEConnectionUpdateCompleteResults 

Structure

# BluetoothHCIEventLEConnectionUpdateCompleteResults

macOS

``` source
struct BluetoothHCIEventLEConnectionUpdateCompleteResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, connInterval: UInt16, connLatency: UInt16, supervisionTimeout: UInt16)

### Instance Properties

var connInterval: UInt16

var connLatency: UInt16

var connectionHandle: BluetoothConnectionHandle

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

