

- Core Telephony
-  CTCarrier Deprecated

Class

# CTCarrier

Information about the user’s cellular service provider, such as its unique identifier and whether it allows VoIP calls on its network.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0Deprecated

``` source
class CTCarrier
```

Deprecated

Deprecated with no replacement

## Topics

### Getting Information About the Cellular Service Provider

var allowsVOIP: Bool

Indicates if the carrier allows making VoIP calls on its network.

var carrierName: String?

The name of the user’s home cellular service provider.

var isoCountryCode: String?

The ISO country code for the user’s cellular service provider.

var mobileCountryCode: String?

The mobile country code (MCC) for the user’s cellular service provider.

var mobileNetworkCode: String?

The mobile network code for the user’s cellular service provider.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Service Information

class CTTelephonyNetworkInfo

An object that provides notifications of changes to the user’s cellular service provider.

