

- Network Extension
- NEHotspotConfiguration
-  init(ssid:passphrase:isWEP:) 

Initializer

# init(ssid:passphrase:isWEP:)

Creates a new hotspot configuration, identified by an SSID, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
init(
    ssid SSID: String,
    passphrase: String,
    isWEP: Bool
)
```

## Parameters 

`SSID`  

The SSID of the WEP or WPA/WPA2 personal Wi-Fi Network. See ssid.

`passphrase`  

The network’s passphrase credential: for WPA or WPA2 personal networks, 8-63 characters; for static 64-bit WEP, 10 hexadecimal digits; for static 128-bit WEP, 26 hexadecimal digits.

`isWEP`  

If `true`, the network is WEP Wi-Fi; otherwise it is a WPA or WPA2 personal Wi-Fi network.

## See Also

### Initializing a configuration

init(ssid: String)

Creates a new hotspot configuration, identified by an SSID, for an open Wi-Fi network.

init(ssid: String, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by an SSID, for a WPA/WPA2 enterprise Wi-Fi network with EAP settings.

init(hs20Settings: NEHotspotHS20Settings, eapSettings: NEHotspotEAPSettings)

Creates a new hotspot configuration, identified by a domain name, for a Hotspot 2.0 Wi-Fi network with HS 2.0 and EAP settings.

init(ssidPrefix: String)

Creates a new hotspot configuration, identified by an SSID prefix string, for an open Wi-Fi network.

init(ssidPrefix: String, passphrase: String, isWEP: Bool)

Creates a new hotspot configuration, identified by an SSID prefix string, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

