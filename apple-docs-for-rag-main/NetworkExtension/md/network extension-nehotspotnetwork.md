

- Network Extension
-  NEHotspotNetwork 

Class

# NEHotspotNetwork

Information about a Wi-Fi network associated with a command or a response.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+visionOS 1.0+watchOS 7.0+

``` source
class NEHotspotNetwork
```

## Overview

When the Hotspot Helper app is asked to evaluate the a network or filter the Wi-Fi scan list, it annotates the `NEHotspotNetwork` object via the `setConfidence:` method.

## Topics

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

enum NEHotspotNetworkSecurityType

An enumeration of constants that define Wi-Fi hotspot network security types.

### Network annotation

func setConfidence(NEHotspotHelperConfidence)

Indicate the level of confidence in being able to handle the network.

enum NEHotspotHelperConfidence

A type that indicates the hotspot helper’s confidence in its ability to handle the network.

func setPassword(String)

Provide the password for a protected network.

### Fetching VPN network information

class func fetchCurrent(completionHandler: (NEHotspotNetwork?) -> Void)

Fetches information about the current Wi-Fi network.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Commands

class NEHotspotHelperCommand

A command for the hotspot helper to handle.

class NEHotspotHelperResponse

The hotspot helper’s response to a command.

