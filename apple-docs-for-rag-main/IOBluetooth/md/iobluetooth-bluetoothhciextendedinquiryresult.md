

- IOBluetooth
-  BluetoothHCIExtendedInquiryResult 

Structure

# BluetoothHCIExtendedInquiryResult

macOS

``` source
struct BluetoothHCIExtendedInquiryResult
```

## Topics

### Initializers

init()

init(numberOfReponses: UInt8, deviceAddress: BluetoothDeviceAddress, pageScanRepetitionMode: BluetoothPageScanRepetitionMode, reserved: UInt8, classOfDevice: BluetoothClassOfDevice, clockOffset: BluetoothClockOffset, RSSIValue: BluetoothHCIRSSIValue, extendedInquiryResponse: BluetoothHCIExtendedInquiryResponse)

### Instance Properties

var RSSIValue: BluetoothHCIRSSIValue

var classOfDevice: BluetoothClassOfDevice

var clockOffset: BluetoothClockOffset

var deviceAddress: BluetoothDeviceAddress

var extendedInquiryResponse: BluetoothHCIExtendedInquiryResponse

var numberOfReponses: UInt8

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

