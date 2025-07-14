

- IOBluetooth
-  BluetoothHCIEventReadRemoteVersionInfoResults 

Structure

# BluetoothHCIEventReadRemoteVersionInfoResults

macOS

``` source
struct BluetoothHCIEventReadRemoteVersionInfoResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, lmpVersion: BluetoothLMPVersion, manufacturerName: BluetoothManufacturerName, lmpSubversion: BluetoothLMPSubversion)

### Instance Properties

var connectionHandle: BluetoothConnectionHandle

var lmpSubversion: BluetoothLMPSubversion

var lmpVersion: BluetoothLMPVersion

var manufacturerName: BluetoothManufacturerName

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

