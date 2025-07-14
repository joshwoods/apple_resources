

- Core WLAN
- CWNetworkProfile
-  ssidData 

Instance Property

# ssidData

The service set identifier (SSID) for the network profile, returned as data.

macOS 10.7+

``` source
var ssidData: Data? { get }
```

## Discussion

The SSID is 1-32 octets.

## See Also

### Instance Properties

var security: CWSecurity

The security mode for the network profile.

var ssid: String?

The service set identifier (SSID) for the network profile, encoded as a string.

