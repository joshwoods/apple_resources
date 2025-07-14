

- DeviceDiscoveryExtension
- DDDevice
-  bluetoothIdentifier 

Instance Property

# bluetoothIdentifier

An identifier to communicate with the device through Bluetooth wireless technology.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
var bluetoothIdentifier: UUID? { get set }
```

## Discussion

An extension may set this property to the Bluetooth identifier of a discovered CBPeripheral.

## See Also

### Indicating the protocol

var `protocol`: DDDevice.Protocol

The manner in which the system applies your app’s device discovery extension.

enum Protocol

An identifier for the manner in which an app interacts with a device.

var protocolType: UTType

A custom universal type that describes the device’s manner of communication with the extension.

var networkEndpoint: NWEndpoint?

An object that describes a local-network device.

