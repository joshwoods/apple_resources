

- Network Extension
- NEAppPushManager
-  matchSSIDs 

Instance Property

# matchSSIDs

An array of Wi-Fi SSID strings that the system matches for local push activation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var matchSSIDs: [String] { get set }
```

## Mentioned in 

Maintaining a Reliable Network Connection

## Discussion

If the SSID string of the current Wi-Fi network matches a member of this array, the framework starts the NEAppPushProvider. The array must contain at least one SSID to start the provider, and has an upper limit of 10 SSIDs.

## See Also

### Matching Wi-Fi networks

var matchPrivateLTENetworks: [NEPrivateLTENetwork]

An array of private LTE networks that the system matches for local push activation.

class NEPrivateLTENetwork

The parameters of a private LTE network.

