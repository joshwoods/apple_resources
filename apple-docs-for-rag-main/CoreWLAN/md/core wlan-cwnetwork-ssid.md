

- Core WLAN
- CWNetwork
-  ssid 

Instance Property

# ssid

The service set identifier (SSID) for the network, encoded as a string.

macOS 10.6+

``` source
var ssid: String? { get }
```

## Discussion

If the SSID can not be encoded as a valid UTF-8 or WinLatin1 string, this method returns *nil*.

## See Also

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

var ssidData: Data?

The service set identifier (SSID) for the network, returned as data.

var wlanChannel: CWChannel?

The channel for the network.

