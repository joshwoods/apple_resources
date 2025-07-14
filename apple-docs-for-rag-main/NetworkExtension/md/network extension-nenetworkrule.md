

- Network Extension
-  NENetworkRule 

Class

# NENetworkRule

A rule to match attributes of network traffic.

macOS 10.15+

``` source
class NENetworkRule
```

## Topics

### Creating a network rule

init(destinationNetwork: NWHostEndpoint, prefix: Int, protocol: NENetworkRule.Protocol)

Creates a rule that matches network traffic destined for a host within a specific network.

Deprecated

init(destinationHost: NWHostEndpoint, protocol: NENetworkRule.Protocol)

Creates a rule that matches network traffic destined for a host within a specific DNS domain.

Deprecated

init(remoteNetwork: NWHostEndpoint?, remotePrefix: Int, localNetwork: NWHostEndpoint?, localPrefix: Int, protocol: NENetworkRule.Protocol, direction: NETrafficDirection)

Creates a rule that matches traffic by remote network, local network, protocol, and direction.

Deprecated

### Matching network traffic characteristics

var matchRemoteEndpoint: NWHostEndpoint?

The remote endpoint that the rule matches.

Deprecated

var matchRemotePrefix: Int

A number that specifies the remote sub-network that the rule matches.

var matchLocalNetwork: NWHostEndpoint?

The local network that the rule matches.

Deprecated

var matchLocalPrefix: Int

A number that specifies the local sub-network that the rule matches.

var matchProtocol: NENetworkRule.Protocol

The protocol that the rule matches.

enum Protocol

A type to represent network protocols used by routing rules.

var matchDirection: NETrafficDirection

The direction of network traffic that the rule matches.

enum NETrafficDirection

A type to represent the direction of network traffic.

### Initializers

convenience init(destinationHostEndpoint: NWEndpoint, protocol: NENetworkRule.Protocol)

convenience init(destinationNetworkEndpoint: NWEndpoint, prefix: Int, protocol: NENetworkRule.Protocol)

convenience init(remoteNetworkEndpoint: NWEndpoint?, remotePrefix: Int, localNetworkEndpoint: NWEndpoint?, localPrefix: Int, protocol: NENetworkRule.Protocol, direction: NETrafficDirection)

### Instance Properties

var matchLocalNetworkEndpoint: NWEndpoint?

var matchRemoteHostOrNetworkEndpoint: NWEndpoint?

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

### Transparent proxy configuration

class NETransparentProxyManager

An object that configures and controls transparent proxies.

class NETransparentProxyProvider

An object that implements the client side of a custom transparent network proxy solution.

class NETransparentProxyNetworkSettings

A specification of what traffic to route through a transparent proxy.

