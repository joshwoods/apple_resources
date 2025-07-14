

- IOBluetooth
-  BluetoothL2CAPCommandRejectReason 

Structure

# BluetoothL2CAPCommandRejectReason

macOS

``` source
struct BluetoothL2CAPCommandRejectReason
```

## Topics

### Constants

var kBluetoothL2CAPCommandRejectReasonCommandNotUnderstood: BluetoothL2CAPCommandRejectReason

var kBluetoothL2CAPCommandRejectReasonInvalidCIDInRequest: BluetoothL2CAPCommandRejectReason

var kBluetoothL2CAPCommandRejectReasonSignallingMTUExceeded: BluetoothL2CAPCommandRejectReason

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

struct BluetoothAMPCommandRejectReason

struct BluetoothAMPCreatePhysicalLinkResponseStatus

struct BluetoothAMPDisconnectPhysicalLinkResponseStatus

struct BluetoothAMPDiscoverResponseControllerStatus

struct BluetoothAMPGetAssocResponseStatus

struct BluetoothAMPGetInfoResponseStatus

struct BluetoothAMPManagerCode

struct BluetoothHCIPowerState

struct BluetoothL2CAPCommandCode

struct BluetoothL2CAPConfigurationOption

struct BluetoothL2CAPConfigurationResult

struct BluetoothL2CAPConfigurationRetransmissionAndFlowControlFlags

struct BluetoothL2CAPConnectionResult

struct BluetoothL2CAPConnectionStatus

struct BluetoothL2CAPInformationExtendedFeaturesMask

