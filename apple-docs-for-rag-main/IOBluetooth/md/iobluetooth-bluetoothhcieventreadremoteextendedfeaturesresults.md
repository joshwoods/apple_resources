

- IOBluetooth
-  BluetoothHCIEventReadRemoteExtendedFeaturesResults 

Structure

# BluetoothHCIEventReadRemoteExtendedFeaturesResults

macOS

``` source
struct BluetoothHCIEventReadRemoteExtendedFeaturesResults
```

## Topics

### Initializers

init()

init(error: BluetoothHCIStatus, connectionHandle: BluetoothConnectionHandle, page: BluetoothHCIPageNumber, maxPage: BluetoothHCIPageNumber, lmpFeatures: BluetoothHCISupportedFeatures)

### Instance Properties

var connectionHandle: BluetoothConnectionHandle

var error: BluetoothHCIStatus

var lmpFeatures: BluetoothHCISupportedFeatures

var maxPage: BluetoothHCIPageNumber

var page: BluetoothHCIPageNumber

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

