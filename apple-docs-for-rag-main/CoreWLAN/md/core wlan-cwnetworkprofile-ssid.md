

- Core WLAN
- CWNetworkProfile
-  ssid 

Instance Property

# ssid

The service set identifier (SSID) for the network profile, encoded as a string.

macOS 10.7+

``` source
var ssid: String? { get }
```

## Discussion

If the SSID can not be encoded as a valid UTF-8 or WinLatin1 string, this method returns *nil*.

## See Also

### Instance Properties

var security: CWSecurity

The security mode for the network profile.

var ssidData: Data?

The service set identifier (SSID) for the network profile, returned as data.

