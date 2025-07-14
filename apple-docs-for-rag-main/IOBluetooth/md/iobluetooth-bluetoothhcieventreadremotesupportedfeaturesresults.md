

- IOBluetooth
-  BluetoothHCIEventReadRemoteSupportedFeaturesResults 

Structure

# BluetoothHCIEventReadRemoteSupportedFeaturesResults

macOS

``` source
struct BluetoothHCIEventReadRemoteSupportedFeaturesResults
```

## Topics

### Initializers

init()

init(error: BluetoothHCIStatus, connectionHandle: BluetoothConnectionHandle, lmpFeatures: BluetoothHCISupportedFeatures)

### Instance Properties

var connectionHandle: BluetoothConnectionHandle

var error: BluetoothHCIStatus

var lmpFeatures: BluetoothHCISupportedFeatures

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

