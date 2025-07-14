

- Network Extension
- NEHotspotConfiguration
-  init(ssid:) 

Initializer

# init(ssid:)

Creates a new hotspot configuration, identified by an SSID, for an open Wi-Fi network.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
init(ssid SSID: String)
```

## Parameters 

`SSID`  

The SSID of the open Wi-Fi network. See ssid.

## See Also

### Initializing a configuration

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

