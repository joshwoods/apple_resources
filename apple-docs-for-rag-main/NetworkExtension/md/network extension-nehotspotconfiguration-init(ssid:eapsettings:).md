

- Network Extension
- NEHotspotConfiguration
-  init(ssid:eapSettings:) 

Initializer

# init(ssid:eapSettings:)

Creates a new hotspot configuration, identified by an SSID, for a WPA/WPA2 enterprise Wi-Fi network with EAP settings.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    ssid SSID: String,
    eapSettings: NEHotspotEAPSettings
)
```

## Parameters 

`SSID`  

The SSID of the WPA/WPA2 enterprise Wi-Fi network. See ssid.

`eapSettings`  

EAP settings. For details, see NEHotspotEAPSettings.

## See Also

### Initializing a configuration

init(ssid: String)

Creates a new hotspot configuration, identified by an SSID, for an open Wi-Fi network.

init(ssid: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

init(hs20Settings: NEHotspotHS20Settings, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by a domain name, for a Hotspot 2.0 Wi-Fi network with HS 2.0 and EAP settings.

init(ssidPrefix: String)

Creates a new hotspot configuration, identified by an SSID prefix string, for an open Wi-Fi network.

init(ssidPrefix: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID prefix string, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

