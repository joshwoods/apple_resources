

- Core WLAN
-  CWNetworkProfile 

Class

# CWNetworkProfile

Encapsulates an immutable network profile entry.

macOS 10.7+

``` source
class CWNetworkProfile
```

## Topics

### Getting a network profile

init()

Creates and returns a CWNetworkProfile object.

init(networkProfile: CWNetworkProfile)

Creates and returns a CWNetworkProfile object initialized with the given CWNetworkProfile object.

### Comparing network profiles

func isEqual(to: CWNetworkProfile) -> Bool

Determine CWNetworkProfile object equality.

### Instance Properties

var security: CWSecurity

The security mode for the network profile.

var ssid: String?

The service set identifier (SSID) for the network profile, encoded as a string.

var ssidData: Data?

The service set identifier (SSID) for the network profile, returned as data.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CWMutableNetworkProfile

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

class CWMutableNetworkProfile

Encapsulates a mutable network profile entry.

class CWNetwork

Encapsulates an IEEE 802.11 network, providing read-only accessors to various properties of the network.

class CWWiFiClient

A wrapper around the entire Wi-Fi subsystem that you use to access interfaces and set up event notifications.

