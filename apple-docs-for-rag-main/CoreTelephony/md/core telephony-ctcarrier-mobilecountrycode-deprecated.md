

- Core Telephony
- CTCarrier
-  mobileCountryCode Deprecated

Instance Property

# mobileCountryCode

The mobile country code (MCC) for the user’s cellular service provider.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
var mobileCountryCode: String? { get }
```

Deprecated

Deprecated; returns '65535' at some point in the future

## Discussion

A read-only NSString object that contains the numeric mobile country code for the user’s cellular service provider. MCCs are defined by ITU-T Recommendation E.212, “List of Mobile Country or Geographical Area Codes”. Typing this property as an NSString object, rather than a number type, preserves leading zeroes in MCCs.

The value for this property is `nil` if any of the following apply:

- There is no SIM card in the device.

- The device is outside of cellular service range.

The value may be `nil` on hardware prior to iPhone 4S when in airplane mode.

## See Also

### Getting Information About the Cellular Service Provider

var allowsVOIP: Bool

Indicates if the carrier allows making VoIP calls on its network.

Deprecated

var carrierName: String?

The name of the user’s home cellular service provider.

Deprecated

var isoCountryCode: String?

The ISO country code for the user’s cellular service provider.

Deprecated

var mobileNetworkCode: String?

The mobile network code for the user’s cellular service provider.

Deprecated

