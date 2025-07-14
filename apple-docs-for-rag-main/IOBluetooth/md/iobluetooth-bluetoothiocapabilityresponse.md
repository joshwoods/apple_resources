

- IOBluetooth
-  BluetoothIOCapabilityResponse 

Structure

# BluetoothIOCapabilityResponse

macOS

``` source
struct BluetoothIOCapabilityResponse
```

## Topics

### Initializers

init()

init(deviceAddress: BluetoothDeviceAddress, ioCapability: BluetoothIOCapability, OOBDataPresence: BluetoothOOBDataPresence, authenticationRequirements: BluetoothAuthenticationRequirements)

### Instance Properties

var OOBDataPresence: BluetoothOOBDataPresence

var authenticationRequirements: BluetoothAuthenticationRequirements

var deviceAddress: BluetoothDeviceAddress

var ioCapability: BluetoothIOCapability

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

