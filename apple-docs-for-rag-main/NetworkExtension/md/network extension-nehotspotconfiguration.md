

- Network Extension
-  NEHotspotConfiguration 

Class

# NEHotspotConfiguration

Configuration settings for a Wi-Fi network.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
class NEHotspotConfiguration
```

## Overview

The `NEHotspotConfiguration` class contains configuration properties and credentials required to connect to Wi-Fi networks.

## Topics

### Initializing a configuration

Create new hotspot configurations for open, WEP, WPA/WPA2 personal, WPA/WPA enterprise, and Hotspot 2.0 Wi-Fi networks.

init(ssid: String)

Creates a new hotspot configuration, identified by an SSID, for an open Wi-Fi network.

init(ssid: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

init(ssid: String, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by an SSID, for a WPA/WPA2 enterprise Wi-Fi network with EAP settings.

init(hs20Settings: NEHotspotHS20Settings, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by a domain name, for a Hotspot 2.0 Wi-Fi network with HS 2.0 and EAP settings.

init(ssidPrefix: String)

Creates a new hotspot configuration, identified by an SSID prefix string, for an open Wi-Fi network.

init(ssidPrefix: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID prefix string, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

### Accessing configuration properties

var ssid: String

The SSID of an open, WEP, WPA/WPA2 personal, or WPA/WPA2 enterprise Wi-Fi network.

var ssidPrefix: String

The string used to match networks against a known SSID prefix.

var lifeTimeInDays: NSNumber

The number of days the network retains the associated configuration.

var joinOnce: Bool

Restricts the lifetime of a configuration to the operating status of the app that created it.

var hidden: Bool

A Boolean value that indicates the visibility of the SSID.

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

class NEHotspotEAPSettings

Extensible Authentication Protocol settings for configuring WPA and WPA2 enterprise Wi-Fi networks.

class NEHotspotHS20Settings

Settings for configuring Hotspot 2.0 Wi-Fi networks.

