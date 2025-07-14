

- Bundle Resources
- Entitlements
-  com.apple.developer.nfc.hce.iso7816.select-identifier-prefixes 

Property List Key

# com.apple.developer.nfc.hce.iso7816.select-identifier-prefixes

An array of identifier strings the app handles with the card session API.

iOS 17.4+iPadOS 17.4+

## Details 

Type  

array of strings

## Discussion

Set this value to include identifier strings for which the app handles ISO7816 `SELECT` requests. You can use a mix of the following identifier types:

- Fully-qualified Application Identifier (AID) strings

- Registered Application Provider Identifier (RID) strings

- Prefix strings that match multiple application identifiers, provided this prefix is at least as long as the RID

To use this entitlement, your app must also have the com.apple.developer.nfc.hce entitlement.

For more information and to apply for this entitlement, visit HCE-based contactless transactions for banking and wallet apps in the European Economic Area.

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

Near Field Communication Tag Reader Session Formats Entitlement

The Near Field Communication data formats an app can read.

**Key:** com.apple.developer.nfc.readersession.formats

com.apple.developer.nfc.hce

A Boolean value indicating whether your app can use the card session API.

com.apple.developer.nfc.hce.default-contactless-app

A Boolean value indicating whether your app can be a default app for contactless NFC with the card session API.

