

- IOBluetooth
-  BluetoothHCIQualityOfServiceSetupParams 

Structure

# BluetoothHCIQualityOfServiceSetupParams

macOS

``` source
struct BluetoothHCIQualityOfServiceSetupParams
```

## Topics

### Initializers

init()

init(flags: UInt8, serviceType: UInt8, tokenRate: UInt32, peakBandwidth: UInt32, latency: UInt32, delayVariation: UInt32)

### Instance Properties

var delayVariation: UInt32

var flags: UInt8

var latency: UInt32

var peakBandwidth: UInt32

var serviceType: UInt8

var tokenRate: UInt32

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

