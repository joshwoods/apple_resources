

- Network Extension
-  NETransparentProxyManager 

Class

# NETransparentProxyManager

An object that configures and controls transparent proxies.

macOS 10.15+

``` source
class NETransparentProxyManager
```

## Topics

### Loading proxy configurations

class func loadAllFromPreferences(completionHandler: ([NETransparentProxyManager]?, (any Error)?) -> Void)

Loads all previously-saved transparent proxy configurations.

## Relationships

### Inherits From

- NEVPNManager

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Transparent proxy configuration

class NETransparentProxyProvider

An object that implements the client side of a custom transparent network proxy solution.

class NETransparentProxyNetworkSettings

A specification of what traffic to route through a transparent proxy.

class NENetworkRule

A rule to match attributes of network traffic.

