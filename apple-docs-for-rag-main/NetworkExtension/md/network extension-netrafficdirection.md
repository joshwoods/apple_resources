

- Network Extension
-  NETrafficDirection 

Enumeration

# NETrafficDirection

A type to represent the direction of network traffic.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum NETrafficDirection
```

## Topics

### Directions

case inbound

The inbound traffic direction.

case outbound

The outbound traffic direction.

case any

A direction that matches either inbound or outbound traffic.

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

enum Protocol

A type to represent network protocols used by routing rules.

var matchDirection: NETrafficDirection

The direction of network traffic that the rule matches.

