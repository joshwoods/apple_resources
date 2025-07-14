

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation
-  network(ssid:credentials:) 

Type Method

# network(ssid:credentials:)

Maintains information about a specific Wi-Fi network.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
static func network(
    ssid: Data,
    credentials: Data
) -> MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation
```

## Parameters 

`ssid`  

The SSID of the Wi-Fi network to associate to.

`credentials`  

The credentials that the sytems requires for associating to that network.

## Discussion

The credentials represent the passphrase that the system needs to associate to the SSID, if one is required. The security type of the Wi-Fi network determines the content of this field, its format, and its valid length.

## See Also

### Getting network information

static var defaultSystemNetwork: MatterAddDeviceExtensionRequestHandler.WiFiNetworkAssociation

The current Wi-Fi network of the iOS device.

