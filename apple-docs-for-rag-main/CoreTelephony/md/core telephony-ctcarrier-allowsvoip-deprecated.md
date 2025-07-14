

- Core Telephony
- CTCarrier
-  allowsVOIP Deprecated

Instance Property

# allowsVOIP

Indicates if the carrier allows making VoIP calls on its network.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
var allowsVOIP: Bool { get }
```

Deprecated

Deprecated; returns YES at some point in the future

## Discussion

A read-only Boolean value that is true if the carrier allows making VoIP calls on its network, or false if not.

If you configure a device for a carrier and then remove the SIM card, this property retains the Boolean value indicating the carrier’s policy regarding VoIP. If you then install a new SIM card, its VoIP policy Boolean replaces the previous value of this property.

## See Also

### Getting Information About the Cellular Service Provider

var carrierName: String?

The name of the user’s home cellular service provider.

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

