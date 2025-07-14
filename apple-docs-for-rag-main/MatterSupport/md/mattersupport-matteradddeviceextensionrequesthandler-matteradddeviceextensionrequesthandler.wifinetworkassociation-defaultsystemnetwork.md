

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation
-  defaultSystemNetwork 

Type Property

# defaultSystemNetwork

The current Wi-Fi network of the iOS device.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
static var defaultSystemNetwork: MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation { get }
```

## See Also

### Getting network information

static func network(ssid: Data, credentials: Data) -> MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

Maintains information about a specific Wi-Fi network.

