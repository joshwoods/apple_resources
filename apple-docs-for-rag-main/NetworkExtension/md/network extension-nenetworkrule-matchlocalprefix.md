

- Network Extension
- NENetworkRule
-  matchLocalPrefix 

Instance Property

# matchLocalPrefix

A number that specifies the local sub-network that the rule matches.

macOS 10.15+

``` source
var matchLocalPrefix: Int { get }
```

## Discussion

This property is NSNotFound for rules whose matchLocalNetwork property is `nil.`

## See Also

### Matching network traffic characteristics

var matchRemoteEndpoint: NWHostEndpoint?

The remote endpoint that the rule matches.

Deprecated

var matchRemotePrefix: Int

A number that specifies the remote sub-network that the rule matches.

var matchLocalNetwork: NWHostEndpoint?

The local network that the rule matches.

Deprecated

var matchProtocol: NENetworkRule.Protocol

The protocol that the rule matches.

enum Protocol

A type to represent network protocols used by routing rules.

var matchDirection: NETrafficDirection

The direction of network traffic that the rule matches.

enum NETrafficDirection

A type to represent the direction of network traffic.

