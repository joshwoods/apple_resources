

- Network Extension
-  NETransparentProxyNetworkSettings 

Class

# NETransparentProxyNetworkSettings

A specification of what traffic to route through a transparent proxy.

macOS 10.15+

``` source
class NETransparentProxyNetworkSettings
```

## Overview

A proxy network settings object contains two properties: an array of rules to include traffic (includedNetworkRules) and an array of rules to exclude traffic (excludedNetworkRules). The exclusion rules take prirority. Therefore, if a given flow matches any of the excludedNetworkRules, evaluation ends and the flow doesn’t route to the proxy. If there’s no match, then evaluation continues and attempts to match the flow against the includedNetworkRules.

## Topics

### Traffic routing rules

var includedNetworkRules: [NENetworkRule]?

An array of rules that collectively specify what traffic to route through the transparent proxy.

var excludedNetworkRules: [NENetworkRule]?

An array of rules that collectively specify what traffic to not route through the transparent proxy.

## Relationships

### Inherits From

- NETunnelNetworkSettings

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

### Transparent proxy configuration

class NETransparentProxyManager

An object that configures and controls transparent proxies.

class NETransparentProxyProvider

An object that implements the client side of a custom transparent network proxy solution.

class NENetworkRule

A rule to match attributes of network traffic.

