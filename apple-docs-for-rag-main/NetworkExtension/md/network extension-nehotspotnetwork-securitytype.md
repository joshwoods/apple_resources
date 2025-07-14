

- Network Extension
- NEHotspotNetwork
-  securityType 

Instance Property

# securityType

The type of security used by the Wi-Fi network.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
var securityType: NEHotspotNetworkSecurityType { get }
```

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

var isChosenHelper: Bool

Indicates whether the calling Hotspot Helper is the chosen helper for this network.

enum NEHotspotNetworkSecurityType

An enumeration of constants that define Wi-Fi hotspot network security types.

