

- Network Extension
-  NEHotspotNetworkSecurityType 

Enumeration

# NEHotspotNetworkSecurityType

An enumeration of constants that define Wi-Fi hotspot network security types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum NEHotspotNetworkSecurityType
```

## Topics

### Security types

case open

A security type to represent an open network with no security protocol.

case WEP

A security type to represent use of Wired Equivalent Privacy (WEP).

case personal

A security type to represent use of Wi-Fi protected access (WPA), WPA2, and WPA3 standards using a pre-shared secret.

case enterprise

A security type to represent use of Wi-Fi protected access (WPA), WPA2, and WPA3 standards using enterprise-level seciurity.

case unknown

A value that represents an unknown security type.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var securityType: NEHotspotNetworkSecurityType

The type of security used by the Wi-Fi network.

