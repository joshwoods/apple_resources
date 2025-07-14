

- Network Extension
- NEHotspotConfiguration
-  init(ssidPrefix:passphrase:isWEP:) 

Initializer

# init(ssidPrefix:passphrase:isWEP:)

Creates a new hotspot configuration, identified by an SSID prefix string, for a protected WEP or WPA/WPA2 personal Wi-Fi network.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
init(
    ssidPrefix SSIDPrefix: String,
    passphrase: String,
    isWEP: Bool
)
```

## Parameters 

`SSIDPrefix`  

A prefix string to match the SSID of a WPA/WPA2 enterprise Wi-Fi network. This value must be between 3 and 32 characters.

`passphrase`  

The network’s passphrase credential: for WPA or WPA2 personal networks, 8-63 characters; for static 64-bit WEP, 10 hexadecimal digits; for static 128-bit WEP, 26 hexadecimal digits.

`isWEP`  

If true, the network is WEP Wi-Fi; otherwise it is a WPA or WPA2 personal Wi-Fi network.

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

init(ssidPrefix: String)

Creates a new hotspot configuration, identified by an SSID prefix string, for an open Wi-Fi network.

