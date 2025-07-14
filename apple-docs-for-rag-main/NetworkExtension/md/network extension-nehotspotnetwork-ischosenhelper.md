

- Network Extension
- NEHotspotNetwork
-  isChosenHelper 

Instance Property

# isChosenHelper

Indicates whether the calling Hotspot Helper is the chosen helper for this network.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var isChosenHelper: Bool { get }
```

## Discussion

The `NEHotspotNetwork` class must have been instantiated via a call to the `supportedNetworkInterfaces` method in the NEHotspotHelper object. This property is useful for restoring state after the Hotspot Helper application has quit and restarted.

## See Also

### Network information

var ssid: String

The SSID for the Wi-Fi network.

var bssid: String

The BSSID for the Wi-Fi network.

var signalStrength: Double

The recent signal strength for the Wi-Fi network.

var isSecure: Bool

Indicates whether the network is secure

var didAutoJoin: Bool

Indicates whether the network was joined automatically or was joined explicitly by the user.

var didJustJoin: Bool

Indicates whether the network was just joined.

var securityType: NEHotspotNetworkSecurityType

The type of security used by the Wi-Fi network.

enum NEHotspotNetworkSecurityType

An enumeration of constants that define Wi-Fi hotspot network security types.

