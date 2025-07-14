

- DeviceDiscoveryExtension
- DDDevice
-  networkEndpoint 

Instance Property

# networkEndpoint

An object that describes a local-network device.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var networkEndpoint: NWEndpoint? { get set }
```

## Discussion

For the discovery of local-network devices, the extension sets the value of this property to the endpoint of an NWBrowser.Result. When a search over the local network succeeds, the browser passes the newly discovered device into your extension’s browseResultsChangedHandler.

## See Also

### Indicating the protocol

var `protocol`: DDDevice.Protocol

The manner in which the system applies your app’s device discovery extension.

enum Protocol

An identifier for the manner in which an app interacts with a device.

var protocolType: UTType

A custom universal type that describes the device’s manner of communication with the extension.

var bluetoothIdentifier: UUID?

An identifier to communicate with the device through Bluetooth wireless technology.

