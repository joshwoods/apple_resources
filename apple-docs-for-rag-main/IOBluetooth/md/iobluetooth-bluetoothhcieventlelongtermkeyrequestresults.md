

- IOBluetooth
-  BluetoothHCIEventLELongTermKeyRequestResults 

Structure

# BluetoothHCIEventLELongTermKeyRequestResults

macOS

``` source
struct BluetoothHCIEventLELongTermKeyRequestResults
```

## Topics

### Initializers

init()

init(connectionHandle: BluetoothConnectionHandle, randomNumber: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8), ediv: UInt16)

### Instance Properties

var connectionHandle: BluetoothConnectionHandle

var ediv: UInt16

var randomNumber: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

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

