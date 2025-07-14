

- Network Extension
- NENetworkRule
-  NENetworkRule.Protocol 

Enumeration

# NENetworkRule.Protocol

A type to represent network protocols used by routing rules.

macOS 10.15+

``` source
enum `Protocol`
```

## Topics

### Protocols

case TCP

A rule protocol to match TCP traffic.

case UDP

A rule protocol to match UDP traffic.

case any

A rule protocol to match TCP and UDP traffic.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var matchLocalPrefix: Int

A number that specifies the local sub-network that the rule matches.

var matchProtocol: NENetworkRule.Protocol

The protocol that the rule matches.

var matchDirection: NETrafficDirection

The direction of network traffic that the rule matches.

enum NETrafficDirection

A type to represent the direction of network traffic.

