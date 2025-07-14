

- IOBluetooth
-  BluetoothL2CAPConnectionResult 

Structure

# BluetoothL2CAPConnectionResult

macOS

``` source
struct BluetoothL2CAPConnectionResult
```

## Topics

### Constants

var kBluetoothL2CAPConnectionResultPending: BluetoothL2CAPConnectionResult

var kBluetoothL2CAPConnectionResultRefusedNoResources: BluetoothL2CAPConnectionResult

var kBluetoothL2CAPConnectionResultRefusedPSMNotSupported: BluetoothL2CAPConnectionResult

var kBluetoothL2CAPConnectionResultRefusedSecurityBlock: BluetoothL2CAPConnectionResult

var kBluetoothL2CAPConnectionResultSuccessful: BluetoothL2CAPConnectionResult

var kBluetoothL2CAPConnectionResultRefusedInvalidSourceCID: BluetoothL2CAPConnectionResult

var kBluetoothL2CAPConnectionResultRefusedReserved: BluetoothL2CAPConnectionResult

var kBluetoothL2CAPConnectionResultRefusedSourceCIDAlreadyAllocated: BluetoothL2CAPConnectionResult

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

struct BluetoothL2CAPCommandRejectReason

struct BluetoothL2CAPConfigurationOption

struct BluetoothL2CAPConfigurationResult

struct BluetoothL2CAPConfigurationRetransmissionAndFlowControlFlags

struct BluetoothL2CAPConnectionStatus

struct BluetoothL2CAPInformationExtendedFeaturesMask

