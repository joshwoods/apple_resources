

- Network Extension
- NEHotspotNetwork
-  isSecure 

Instance Property

# isSecure

Indicates whether the network is secure

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var isSecure: Bool { get }
```

## See Also

### Network information

var ssid: String

The SSID for the Wi-Fi network.

var bssid: String

The BSSID for the Wi-Fi network.

var signalStrength: Double

The recent signal strength for the Wi-Fi network.

var didAutoJoin: Bool

Indicates whether the network was joined automatically or was joined explicitly by the user.

var didJustJoin: Bool

Indicates whether the network was just joined.

var isChosenHelper: Bool

Indicates whether the calling Hotspot Helper is the chosen helper for this network.

var securityType: NEHotspotNetworkSecurityType

The type of security used by the Wi-Fi network.

enum NEHotspotNetworkSecurityType

An enumeration of constants that define Wi-Fi hotspot network security types.

