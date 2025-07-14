

- Network Extension
-  NEHotspotHS20Settings 

Class

# NEHotspotHS20Settings

Settings for configuring Hotspot 2.0 Wi-Fi networks.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEHotspotHS20Settings
```

## Topics

### Initializing Hotspot 2.0 settings

init(domainName: String, roamingEnabled: Bool)

Creates a new hotspot configuration of a legacy Hotspot or HS 2.0 Wi-Fi network. with optional roaming enabled.

### Accessing Hotspot 2.0 properties

var domainName: String

The domain name of a Hotspot 2.0 Wi-Fi Network.

var isRoamingEnabled: Bool

A Boolean value indicating whether or not roaming is enabled on a Hotspot 2.0 Wi-Fi network.

var mccAndMNCs: [String]

An array of Mobile Country Code (MCC) and Mobile Network Code (MNC) pairs used for Wi-Fi Hotspot 2.0 negotiation.

var naiRealmNames: [String]

An array of Network Access Identifier (NAI) realm name strings used for Wi-Fi Hotspot 2.0 negotiation.

var roamingConsortiumOIs: [String]

An array of Roaming Consortium Organization (RCO) identifiers used for Wi-Fi Hotspot 2.0 negotiation.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Wi-Fi network configuration

class NEHotspotConfigurationManager

A manager that applies and removes hotspot configurations of Wi-Fi networks.

class NEHotspotConfiguration

Configuration settings for a Wi-Fi network.

class NEHotspotEAPSettings

Extensible Authentication Protocol settings for configuring WPA and WPA2 enterprise Wi-Fi networks.

