

- Bundle Resources
- Entitlements
-  Multipath Entitlement 

Property List Key

# Multipath Entitlement

A Boolean value indicating whether your app may use Multipath protocols to seamlessly transition between Wi-Fi and cellular networks.

iOS 3.0+iPadOS 3.0+visionOS 1.0+

## Details 

Key  
com.apple.developer.networking.multipath

Type  

boolean

## Discussion

This key Indicates whether your app may use Multipath protocols, such as Multipath TCP, to smoothly hand over traffic from one interface to another.

To add this entitlement to your app, enable the Multipath capability in Xcode.

## See Also

### Related Documentation

Improving network reliability using Multipath TCP

Use the available radios in iOS devices to improve your app’s network reliability and performance.

enum URLSessionConfiguration.MultipathServiceType

Constants that specify the type of service that Multipath TCP uses.

### Wireless interfaces

Access Wi-Fi Information Entitlement

A Boolean value indicating whether your app can access information about the connected Wi-Fi network.

**Key:** com.apple.developer.networking.wifi-info

Wireless Accessory Configuration Entitlement

A Boolean value that indicates whether your app may configure MFi Wi-Fi accessories.

**Key:** com.apple.external-accessory.wireless-configuration

Hotspot Configuration Entitlement

A Boolean value indicating whether your app can use the hotspot manager to configure Wi-Fi networks.

**Key:** com.apple.developer.networking.HotspotConfiguration

Near Field Communication Tag Reader Session Formats Entitlement

The Near Field Communication data formats an app can read.

**Key:** com.apple.developer.nfc.readersession.formats

com.apple.developer.nfc.hce

A Boolean value indicating whether your app can use the card session API.

com.apple.developer.nfc.hce.iso7816.select-identifier-prefixes

An array of identifier strings the app handles with the card session API.

com.apple.developer.nfc.hce.default-contactless-app

A Boolean value indicating whether your app can be a default app for contactless NFC with the card session API.

