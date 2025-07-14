

- Network Extension
- NEHotspotConfiguration
-  hidden 

Instance Property

# hidden

A Boolean value that indicates the visibility of the SSID.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
var hidden: Bool { get set }
```

## Discussion

Set this value to true to make the system perform an active scan for the Service Set Identifier (SSID). If the access point is already broadcasting the SSID, set this value to false.

The default value is false.

## See Also

### Accessing configuration properties

var ssid: String

The SSID of an open, WEP, WPA/WPA2 personal, or WPA/WPA2 enterprise Wi-Fi network.

var ssidPrefix: String

The string used to match networks against a known SSID prefix.

var lifeTimeInDays: NSNumber

The number of days the network retains the associated configuration.

var joinOnce: Bool

Restricts the lifetime of a configuration to the operating status of the app that created it.

