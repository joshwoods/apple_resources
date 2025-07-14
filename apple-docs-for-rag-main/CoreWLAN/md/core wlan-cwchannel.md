

- Core WLAN
-  CWChannel 

Class

# CWChannel

Encapsulates an IEEE 802.11 channel.

macOS 10.7+

``` source
class CWChannel
```

## Topics

### Comparing channels

func isEqual(to: CWChannel) -> Bool

Determine CWChannel object equality.

### Instance Properties

var channelBand: CWChannelBand

The channel band.

var channelNumber: Int

The channel number.

var channelWidth: CWChannelWidth

The channel width.

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

### Classes

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

class CWNetworkProfile

Encapsulates an immutable network profile entry.

class CWWiFiClient

A wrapper around the entire Wi-Fi subsystem that you use to access interfaces and set up event notifications.

