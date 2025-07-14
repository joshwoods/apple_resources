

- IOBluetooth
-  BluetoothHCIEnhancedSetupSynchronousConnectionParams 

Structure

# BluetoothHCIEnhancedSetupSynchronousConnectionParams

macOS

``` source
struct BluetoothHCIEnhancedSetupSynchronousConnectionParams
```

## Topics

### Initializers

init()

init(transmitBandwidth: UInt32, receiveBandwidth: UInt32, transmitCodingFormat: UInt64, receiveCodingFormat: UInt64, transmitCodecFrameSize: UInt16, receiveCodecFrameSize: UInt16, inputBandwidth: UInt32, outputBandwidth: UInt32, inputCodingFormat: UInt64, outputCodingFormat: UInt64, inputCodedDataSize: UInt16, outputCodedDataSize: UInt16, inputPCMDataFormat: UInt8, outputPCMDataFormat: UInt8, inputPCMSamplePayloadMSBPosition: UInt8, outputPCMSamplePayloadMSBPosition: UInt8, inputDataPath: UInt8, outputDataPath: UInt8, inputTransportUnitSize: UInt8, outputTransportUnitSize: UInt8, maxLatency: UInt16, packetType: UInt16, retransmissionEffort: UInt8)

### Instance Properties

var inputBandwidth: UInt32

var inputCodedDataSize: UInt16

var inputCodingFormat: UInt64

var inputDataPath: UInt8

var inputPCMDataFormat: UInt8

var inputPCMSamplePayloadMSBPosition: UInt8

var inputTransportUnitSize: UInt8

var maxLatency: UInt16

var outputBandwidth: UInt32

var outputCodedDataSize: UInt16

var outputCodingFormat: UInt64

var outputDataPath: UInt8

var outputPCMDataFormat: UInt8

var outputPCMSamplePayloadMSBPosition: UInt8

var outputTransportUnitSize: UInt8

var packetType: UInt16

var receiveBandwidth: UInt32

var receiveCodecFrameSize: UInt16

var receiveCodingFormat: UInt64

var retransmissionEffort: UInt8

var transmitBandwidth: UInt32

var transmitCodecFrameSize: UInt16

var transmitCodingFormat: UInt64

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

