

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.ThreadScanResult
-  extendedAddress 

Instance Property

# extendedAddress

The identifier of an active Thread network Border Agent.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
var extendedAddress: Data
```

## Discussion

This corresponds to the Border Agent ID in retrieveCredentials(forBorderAgent:completion:).

## See Also

### Getting result information

var channel: UInt16

The Thread network radio channel.

var extendedPANID: UInt64

The Thread network extended PAN identifier.

var linkQualityIndicator: UInt8

A receive quality indicator, as specified by Matter specification.

var networkName: String

The Thread network name.

var panID: UInt16

The Thread network PAN identifier.

var rssi: Int8

The observed RSSI of the network by the device.

var version: UInt8

The version field, as specified by the Matter specificaiton.

