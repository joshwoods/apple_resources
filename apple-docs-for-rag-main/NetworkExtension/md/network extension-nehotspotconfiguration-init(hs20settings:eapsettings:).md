

- Network Extension
- NEHotspotConfiguration
-  init(hs20Settings:eapSettings:) 

Initializer

# init(hs20Settings:eapSettings:)

Creates a new hotspot configuration, identified by a domain name, for a Hotspot 2.0 Wi-Fi network with HS 2.0 and EAP settings.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    hs20Settings: NEHotspotHS20Settings,
    eapSettings: NEHotspotEAPSettings
)
```

## Parameters 

`hs20Settings`  

Hotspot 2.0 settings. For possible values, see NEHotspotHS20Settings.

`eapSettings`  

EAP settings. For possible values, see NEHotspotEAPSettings

## See Also

### Initializing a configuration

init(ssid: String)

Creates a new hotspot configuration, identified by an SSID, for an open Wi-Fi network.

init(ssid: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

init(ssid: String, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by an SSID, for a WPA/WPA2 enterprise Wi-Fi network with EAP settings.

init(ssidPrefix: String)

Creates a new hotspot configuration, identified by an SSID prefix string, for an open Wi-Fi network.

init(ssidPrefix: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID prefix string, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

