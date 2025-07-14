

- IOBluetooth
-  BluetoothHCIVersionInfo 

Structure

# BluetoothHCIVersionInfo

macOS

``` source
struct BluetoothHCIVersionInfo
```

## Topics

### Initializers

init()

init(manufacturerName: BluetoothManufacturerName, lmpVersion: BluetoothLMPVersion, lmpSubVersion: BluetoothLMPSubversion, hciVersion: UInt8, hciRevision: UInt16)

### Instance Properties

var hciRevision: UInt16

var hciVersion: UInt8

var lmpSubVersion: BluetoothLMPSubversion

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

