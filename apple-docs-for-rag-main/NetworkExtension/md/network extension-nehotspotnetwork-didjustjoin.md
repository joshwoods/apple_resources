

- Network Extension
- NEHotspotNetwork
-  didJustJoin 

Instance Property

# didJustJoin

Indicates whether the network was just joined.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var didJustJoin: Bool { get }
```

## Discussion

This property is useful in the Maintaining state to differentiate whether the Maintain command is for the initial join, or the subsequent periodic callback.

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

var isChosenHelper: Bool

Indicates whether the calling Hotspot Helper is the chosen helper for this network.

var securityType: NEHotspotNetworkSecurityType

The type of security used by the Wi-Fi network.

enum NEHotspotNetworkSecurityType

An enumeration of constants that define Wi-Fi hotspot network security types.

