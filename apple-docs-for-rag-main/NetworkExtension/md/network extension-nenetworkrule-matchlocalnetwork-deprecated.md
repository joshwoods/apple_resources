

- Network Extension
- NENetworkRule
-  matchLocalNetwork Deprecated

Instance Property

# matchLocalNetwork

The local network that the rule matches.

macOS 10.15–15.0Deprecated

``` source
var matchLocalNetwork: NWHostEndpoint? { get }
```

## See Also

### Matching network traffic characteristics

var matchRemoteEndpoint: NWHostEndpoint?

The remote endpoint that the rule matches.

Deprecated

var matchRemotePrefix: Int

A number that specifies the remote sub-network that the rule matches.

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

