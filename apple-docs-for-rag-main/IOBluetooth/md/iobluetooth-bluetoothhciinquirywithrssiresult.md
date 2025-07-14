

- IOBluetooth
-  BluetoothHCIInquiryWithRSSIResult 

Structure

# BluetoothHCIInquiryWithRSSIResult

macOS

``` source
struct BluetoothHCIInquiryWithRSSIResult
```

## Topics

### Initializers

init()

init(deviceAddress: BluetoothDeviceAddress, pageScanRepetitionMode: BluetoothPageScanRepetitionMode, reserved: UInt8, classOfDevice: BluetoothClassOfDevice, clockOffset: BluetoothClockOffset, RSSIValue: BluetoothHCIRSSIValue)

### Instance Properties

var RSSIValue: BluetoothHCIRSSIValue

var classOfDevice: BluetoothClassOfDevice

var clockOffset: BluetoothClockOffset

var deviceAddress: BluetoothDeviceAddress

var pageScanRepetitionMode: BluetoothPageScanRepetitionMode

var reserved: UInt8

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

