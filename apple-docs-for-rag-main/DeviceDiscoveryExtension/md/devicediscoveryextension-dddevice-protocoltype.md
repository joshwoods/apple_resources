

- DeviceDiscoveryExtension
- DDDevice
-  protocolType 

Instance Property

# protocolType

A custom universal type that describes the device’s manner of communication with the extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
var protocolType: UTType { get set }
```

## See Also

### Indicating the protocol

var `protocol`: DDDevice.Protocol

The manner in which the system applies your app’s device discovery extension.

enum Protocol

An identifier for the manner in which an app interacts with a device.

var bluetoothIdentifier: UUID?

An identifier to communicate with the device through Bluetooth wireless technology.

var networkEndpoint: NWEndpoint?

An object that describes a local-network device.

