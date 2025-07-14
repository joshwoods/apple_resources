

- IOBluetooth
-  BluetoothHCIEventFlowSpecificationData 

Structure

# BluetoothHCIEventFlowSpecificationData

macOS

``` source
struct BluetoothHCIEventFlowSpecificationData
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, flags: UInt8, flowDirection: UInt8, serviceType: UInt8, tokenRate: UInt32, tokenBucketSize: UInt32, peakBandwidth: UInt32, accessLatency: UInt32)

### Instance Properties

var accessLatency: UInt32

var connectionHandle: BluetoothConnectionHandle

var flags: UInt8

var flowDirection: UInt8

var peakBandwidth: UInt32

var serviceType: UInt8

var tokenBucketSize: UInt32

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

