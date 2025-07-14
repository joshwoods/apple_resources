

- DeviceDiscoveryExtension
- DDDevice
-  protocol 

Instance Property

# protocol

The manner in which the system applies your app’s device discovery extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
var `protocol`: DDDevice.Protocol { get set }
```

## Discussion

The value is DDDevice.Protocol.dial for the discovery of third-party media receivers.

## See Also

### Indicating the protocol

enum Protocol

An identifier for the manner in which an app interacts with a device.

var protocolType: UTType

A custom universal type that describes the device’s manner of communication with the extension.

var bluetoothIdentifier: UUID?

An identifier to communicate with the device through Bluetooth wireless technology.

var networkEndpoint: NWEndpoint?

An object that describes a local-network device.

