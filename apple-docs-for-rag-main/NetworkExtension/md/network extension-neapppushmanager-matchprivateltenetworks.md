

- Network Extension
- NEAppPushManager
-  matchPrivateLTENetworks 

Instance Property

# matchPrivateLTENetworks

An array of private LTE networks that the system matches for local push activation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var matchPrivateLTENetworks: [NEPrivateLTENetwork] { get set }
```

## Discussion

If the properties of current private LTE network matches with the properties of a member of this array then the system starts the NEAppPushProvider. The array must contain at least one SSID to start the provider, and has an upper limit of 10 private LTE networks. For private LTE networks that aren’t band 48, only supervised devices can perform the match.

## See Also

### Matching Wi-Fi networks

var matchSSIDs: [String]

An array of Wi-Fi SSID strings that the system matches for local push activation.

class NEPrivateLTENetwork

The parameters of a private LTE network.

