

- Network
- NWProtocolQUIC
- NWProtocolQUIC.Metadata
-  NWProtocolQUIC.Metadata.KeepAliveBehavior 

Enumeration

# NWProtocolQUIC.Metadata.KeepAliveBehavior

A QUIC connection keepalive behavior.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum KeepAliveBehavior
```

## Topics

### Keepalive Behaviors

case on

Keepalives are enabled with the default timeout.

case off

Keepalives are disabled.

case seconds(Int)

Keepalives are enabled with a custom timeout, in seconds.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring Keepalives

var keepAlive: NWProtocolQUIC.Metadata.KeepAliveBehavior

The QUIC connection keepalive behavior.

