

- DeviceDiscoveryExtension
- DDDevice
-  url 

Instance Property

# url

A resource locator for the simple service discovery protocol.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
var url: URL { get set }
```

## Discussion

Set this property to indicate communication with a device over the simple service discovery protocol (SSDP). The value needs to:

- Resolve to a valid hostname.

- Include no query parameters.

- Be of a size no greater than 100 bytes.

## See Also

### Setting the device state

var state: DDDeviceState

A state that represents the level of user interaction with the device.

var txtRecord: NWTXTRecord?

A dictionary of metadata for the device that the extension communicates with over the local network.

var supportsGrouping: Bool

A Boolean value that indicates whether to group the device with others in the AirPlay UI.

