

- Bundle Resources
- Entitlements
-  Wireless Accessory Configuration Entitlement 

Property List Key

# Wireless Accessory Configuration Entitlement

A Boolean value that indicates whether your app may configure MFi Wi-Fi accessories.

iOS 3.0+iPadOS 3.0+

## Details 

Key  
com.apple.external-accessory.wireless-configuration

Type  

boolean

## Discussion

This key indicates whether your app may configure third-party hardware accessories that use Apple’s MFi licensed technology to connect to Apple devices.

To add this entitlement to your app, enable the Wireless Accessory Configuration capability in Xcode.

## See Also

### Related Documentation

External Accessory

Communicate with accessories that connect to a device with the Apple Lightning connector, or with Bluetooth wireless technology.

### Wireless interfaces

Access Wi-Fi Information Entitlement

A Boolean value indicating whether your app can access information about the connected Wi-Fi network.

**Key:** com.apple.developer.networking.wifi-info

Multipath Entitlement

A Boolean value indicating whether your app may use Multipath protocols to seamlessly transition between Wi-Fi and cellular networks.

**Key:** com.apple.developer.networking.multipath

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

