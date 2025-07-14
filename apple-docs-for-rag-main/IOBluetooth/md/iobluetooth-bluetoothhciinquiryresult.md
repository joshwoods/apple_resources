

- IOBluetooth
-  BluetoothHCIInquiryResult 

Structure

# BluetoothHCIInquiryResult

macOS

``` source
struct BluetoothHCIInquiryResult
```

## Topics

### Initializers

init()

init(deviceAddress: BluetoothDeviceAddress, pageScanRepetitionMode: BluetoothPageScanRepetitionMode, pageScanPeriodMode: BluetoothHCIPageScanPeriodMode, pageScanMode: BluetoothHCIPageScanMode, classOfDevice: BluetoothClassOfDevice, clockOffset: BluetoothClockOffset)

### Instance Properties

var classOfDevice: BluetoothClassOfDevice

var clockOffset: BluetoothClockOffset

var deviceAddress: BluetoothDeviceAddress

var pageScanMode: BluetoothHCIPageScanMode

var pageScanPeriodMode: BluetoothHCIPageScanPeriodMode

var pageScanRepetitionMode: BluetoothPageScanRepetitionMode

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

