

- Core WLAN
-  CWMutableNetworkProfile 

Class

# CWMutableNetworkProfile

Encapsulates a mutable network profile entry.

macOS 10.7+

``` source
class CWMutableNetworkProfile
```

## Overview

Use this class to change profile properties. To commit Wi-Fi network profile changes, use networkProfiles and commitConfiguration(_:authorization:).

## Topics

### Configuring Network Profiles

var ssidData: Data?

The service set identifier (SSID).

var security: CWSecurity

The security type.

## Relationships

### Inherits From

- CWNetworkProfile

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Classes

class CWChannel

Encapsulates an IEEE 802.11 channel.

class CWConfiguration

Encapsulates an immutable configuration for an AirPort WLAN interface.

class CWInterface

Encapsulates an IEEE 802.11 interface.

class CWMutableConfiguration

Encapsulates a mutable configuration for an AirPort WLAN interface.

class CWNetwork

Encapsulates an IEEE 802.11 network, providing read-only accessors to various properties of the network.

class CWNetworkProfile

Encapsulates an immutable network profile entry.

class CWWiFiClient

A wrapper around the entire Wi-Fi subsystem that you use to access interfaces and set up event notifications.

