

- Core Telephony
- CTCarrier
-  carrierName Deprecated

Instance Property

# carrierName

The name of the user’s home cellular service provider.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
var carrierName: String? { get }
```

Deprecated

Deprecated; returns '--' at some point in the future

## Discussion

The carrier provides this string, formatting it for presentation to the user. The value does not change if the user is roaming; it always represents the provider with which the user has an account.

If you configure a device for a carrier and then remove the SIM card, this property retains the name of the carrier. If you then install a new SIM card, its carrier name replaces the previous value of this property.

The value for this property is `nil` if the user never configured a carrier for the device.

## See Also

### Getting Information About the Cellular Service Provider

var allowsVOIP: Bool

Indicates if the carrier allows making VoIP calls on its network.

Deprecated

var isoCountryCode: String?

The ISO country code for the user’s cellular service provider.

Deprecated

var mobileCountryCode: String?

The mobile country code (MCC) for the user’s cellular service provider.

Deprecated

var mobileNetworkCode: String?

The mobile network code for the user’s cellular service provider.

Deprecated

