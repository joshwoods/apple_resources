

- Network Extension
- NENetworkRule
-  matchRemotePrefix 

Instance Property

# matchRemotePrefix

A number that specifies the remote sub-network that the rule matches.

macOS 10.15+

``` source
var matchRemotePrefix: Int { get }
```

## Discussion

This property is NSNotFound for rules where matchRemoteEndpoint doesn’t contain an IP address.

## See Also

### Matching network traffic characteristics

var matchRemoteEndpoint: NWHostEndpoint?

The remote endpoint that the rule matches.

Deprecated

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

