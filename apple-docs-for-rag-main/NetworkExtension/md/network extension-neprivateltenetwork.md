

- Network Extension
-  NEPrivateLTENetwork 

Class

# NEPrivateLTENetwork

The parameters of a private LTE network.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
class NEPrivateLTENetwork
```

## Overview

Populate your manager’s matchPrivateLTENetworks with an array of objects of this type. The system starts the provider when the device’s current private LTE provider matches the properties of any member of the array.

## Topics

### Accessing network properties

var mobileCountryCode: String

The Mobile Country Code (MCC) of the private LTE network.

var mobileNetworkCode: String

The Mobile Network Code (MNC) of the private LTE network.

var trackingAreaCode: String?

The Tracking Area Code of the private LTE network.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Matching Wi-Fi networks

var matchSSIDs: [String]

An array of Wi-Fi SSID strings that the system matches for local push activation.

var matchPrivateLTENetworks: [NEPrivateLTENetwork]

An array of private LTE networks that the system matches for local push activation.

