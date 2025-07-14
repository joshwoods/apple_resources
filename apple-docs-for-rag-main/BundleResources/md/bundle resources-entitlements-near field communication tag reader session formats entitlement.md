

- Bundle Resources
- Entitlements
-  Near Field Communication Tag Reader Session Formats Entitlement 

Property List Key

# Near Field Communication Tag Reader Session Formats Entitlement

The Near Field Communication data formats an app can read.

iOS 11.0+iPadOS 11.0+

## Details 

Key  
com.apple.developer.nfc.readersession.formats

Type  

array of strings

## Possible Values 

`TAG`  

Allows read and write access to a tag using NFCTagReaderSession.

## Discussion

To add this entitlement to your app, enable the Near Field Communication Tag Reading capability in Xcode.

## See Also

### Wireless interfaces

Access Wi-Fi Information Entitlement

A Boolean value indicating whether your app can access information about the connected Wi-Fi network.

**Key:** com.apple.developer.networking.wifi-info

Wireless Accessory Configuration Entitlement

A Boolean value that indicates whether your app may configure MFi Wi-Fi accessories.

**Key:** com.apple.external-accessory.wireless-configuration

Multipath Entitlement

A Boolean value indicating whether your app may use Multipath protocols to seamlessly transition between Wi-Fi and cellular networks.

**Key:** com.apple.developer.networking.multipath

Hotspot Configuration Entitlement

A Boolean value indicating whether your app can use the hotspot manager to configure Wi-Fi networks.

**Key:** com.apple.developer.networking.HotspotConfiguration

com.apple.developer.nfc.hce

A Boolean value indicating whether your app can use the card session API.

com.apple.developer.nfc.hce.iso7816.select-identifier-prefixes

An array of identifier strings the app handles with the card session API.

com.apple.developer.nfc.hce.default-contactless-app

A Boolean value indicating whether your app can be a default app for contactless NFC with the card session API.

