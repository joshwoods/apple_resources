

- Core Telephony
- CTCarrier
-  isoCountryCode Deprecated

Instance Property

# isoCountryCode

The ISO country code for the user’s cellular service provider.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
var isoCountryCode: String? { get }
```

Deprecated

Deprecated; returns '--' at some point in the future

## Discussion

This property uses the ISO 3166-1 country code representation.

The value for this property is `nil` if any of the following apply:

- The device is in airplane mode.

- There is no SIM card in the device.

- The device is outside of cellular service range.

## See Also

### Getting Information About the Cellular Service Provider

var allowsVOIP: Bool

Indicates if the carrier allows making VoIP calls on its network.

Deprecated

var carrierName: String?

The name of the user’s home cellular service provider.

Deprecated

var mobileCountryCode: String?

The mobile country code (MCC) for the user’s cellular service provider.

Deprecated

var mobileNetworkCode: String?

The mobile network code for the user’s cellular service provider.

Deprecated

