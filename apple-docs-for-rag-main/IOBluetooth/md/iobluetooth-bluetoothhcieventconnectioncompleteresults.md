

- IOBluetooth
-  BluetoothHCIEventConnectionCompleteResults 

Structure

# BluetoothHCIEventConnectionCompleteResults

macOS

``` source
struct BluetoothHCIEventConnectionCompleteResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, deviceAddress: BluetoothDeviceAddress, linkType: BluetoothLinkType, encryptionMode: BluetoothHCIEncryptionMode)

### Instance Properties

var connectionHandle: BluetoothConnectionHandle

var deviceAddress: BluetoothDeviceAddress

var encryptionMode: BluetoothHCIEncryptionMode

var linkType: BluetoothLinkType

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

