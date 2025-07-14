

- Core WLAN
-  CWNetwork 

Class

# CWNetwork

Encapsulates an IEEE 802.11 network, providing read-only accessors to various properties of the network.

macOS 10.6+

``` source
class CWNetwork
```

## Topics

### Getting supported security types

func supportsSecurity(CWSecurity) -> Bool

Method for determining which security types a network supports.

### Getting supported PHY modes

func supportsPHYMode(CWPHYMode) -> Bool

Method for determining which PHY modes a network supports.

### Comparing wireless networks

func isEqual(to: CWNetwork) -> Bool

Method for determining CWNetwork object equality.

### Instance Properties

var beaconInterval: Int

The beacon interval (ms) for the network.

var bssid: String?

The basic service set identifier (BSSID) for the network, returned as UTF-8 string.

var countryCode: String?

The country code (ISO/IEC 3166-1:1997) for the network.

var ibss: Bool

The network is an IBSS network.

var informationElementData: Data?

Information element data included in beacon or probe response frames.

var noiseMeasurement: Int

The aggregate noise measurement (dBm) for the network.

var rssiValue: Int

The aggregate received signal strength indication (RSSI) measurement (dBm) for the network.

var ssid: String?

The service set identifier (SSID) for the network, encoded as a string.

var ssidData: Data?

The service set identifier (SSID) for the network, returned as data.

var wlanChannel: CWChannel?

The channel for the network.

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

class CWNetworkProfile

Encapsulates an immutable network profile entry.

class CWWiFiClient

A wrapper around the entire Wi-Fi subsystem that you use to access interfaces and set up event notifications.

