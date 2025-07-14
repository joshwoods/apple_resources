

- IOBluetooth
-  IOBluetoothL2CAPChannelEvent 

Structure

# IOBluetoothL2CAPChannelEvent

macOS

``` source
struct IOBluetoothL2CAPChannelEvent
```

## Topics

### Initializers

init()

init(eventType: IOBluetoothL2CAPChannelEventType, u: IOBluetoothL2CAPChannelEvent.__Unnamed_union_u, status: IOReturn)

### Instance Properties

var eventType: IOBluetoothL2CAPChannelEventType

var status: IOReturn

var u: IOBluetoothL2CAPChannelEvent.__Unnamed_union_u

## Relationships

### Conforms To

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

