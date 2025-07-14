

- Network
- NWConnection
- NWConnection.EstablishmentReport
-  NWConnection.EstablishmentReport.Handshake 

Structure

# NWConnection.EstablishmentReport.Handshake

A description of a single protocol handshake.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Handshake
```

## Topics

### Measuring Performance

let handshakeDuration: TimeInterval

The duration of the protocol handshake.

let handshakeRTT: TimeInterval

The round-trip time the protocol observed during its handshake.

### Identifying Protocols

let definition: NWProtocolDefinition

The protocol performing the handshake.

## Relationships

### Conforms To

- Sendable

## See Also

### Inspecting Protocol Handshakes

let handshakes: [NWConnection.EstablishmentReport.Handshake]

The array of protocol handshakes in order from first completed to last completed.

