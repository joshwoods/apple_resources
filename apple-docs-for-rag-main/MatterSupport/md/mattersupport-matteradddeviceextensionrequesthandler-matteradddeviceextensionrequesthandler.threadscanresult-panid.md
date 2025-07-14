

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.ThreadScanResult
-  panID 

Instance Property

# panID

The Thread network PAN identifier.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
var panID: UInt16
```

## See Also

### Getting result information

var channel: UInt16

The Thread network radio channel.

var extendedAddress: Data

The identifier of an active Thread network Border Agent.

var extendedPANID: UInt64

The Thread network extended PAN identifier.

var linkQualityIndicator: UInt8

A receive quality indicator, as specified by Matter specification.

var networkName: String

The Thread network name.

var rssi: Int8

The observed RSSI of the network by the device.

var version: UInt8

The version field, as specified by the Matter specificaiton.

