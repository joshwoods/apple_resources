

- DeviceDiscoveryExtension
- DDDevice
-  txtRecord 

Instance Property

# txtRecord

A dictionary of metadata for the device that the extension communicates with over the local network.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var txtRecord: NWTXTRecord? { get set }
```

## Discussion

Particularly, this dictionary provides the human-readable device name with its `“NAME”` key.

## See Also

### Setting the device state

var state: DDDeviceState

A state that represents the level of user interaction with the device.

var url: URL

A resource locator for the simple service discovery protocol.

var supportsGrouping: Bool

A Boolean value that indicates whether to group the device with others in the AirPlay UI.

