

- Network Extension
- NEHotspotConfiguration
-  init(ssidPrefix:) 

Initializer

# init(ssidPrefix:)

Creates a new hotspot configuration, identified by an SSID prefix string, for an open Wi-Fi network.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
init(ssidPrefix SSIDPrefix: String)
```

## Parameters 

`SSIDPrefix`  

A prefix string to match the SSID of an open Wi-Fi Network. This value must be between 3 and 32 characters.

## Discussion

Use this initializer when you want to match a known SSID prefix, but don’t have a full SSID. If the system finds multiple Wi-Fi networks whose SSID string matches the given prefix, it selects the network with the greatest signal strength.

## See Also

### Initializing a configuration

init(ssid: String)

Creates a new hotspot configuration, identified by an SSID, for an open Wi-Fi network.

init(ssid: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

init(ssid: String, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by an SSID, for a WPA/WPA2 enterprise Wi-Fi network with EAP settings.

init(hs20Settings: NEHotspotHS20Settings, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by a domain name, for a Hotspot 2.0 Wi-Fi network with HS 2.0 and EAP settings.

init(ssidPrefix: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID prefix string, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

